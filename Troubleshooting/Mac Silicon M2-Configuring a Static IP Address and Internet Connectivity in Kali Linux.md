# Troubleshooting Internet Connection Issue
I was having trouble getting an internet connection in VirtualBox on my M2 Mac, even though my host system was connected to Wi-Fi. I tried using a Bridged Adapter, but **DHCP completely failed** to assign an IP address. After trying various fixes, I finally resolved it by manually configuring a **static IP** inside the VM.

### 📸 Here, I have attached all the screenshots showing the issues I encountered and the steps I followed to successfully resolve them.
I received valuable guidance and support from my professional instructor.
### Checking IP address
I checked the ip address 
```
ip a
```

<img src="images/1.png" width="500">

---

### Asking IP address
Using dhclient for asking router for IP Address
```
dhclient -v eth0
```
* dhclient = Get IP address
* -v = Show details
* eth0 = Network adapter

<img src="images/5.JPG" width="500">

But as you can see it says command 'dhclient' not found, so need to install **DHCP Client**. 

Steps to Follow: 
```
sudo apt install isc-dhcp-client
```
**This will install DHCP CLient**

```
sudo apt install-dhcp-client-ddns
```

But in my terminal after running first command but Error occurred:failed to fetch the dhcp client 

<img src="images/6.JPG" width="500">

---

### Trying to reach another device over same network 
For that need i tried 
```
ping 8.8.8.8
```
<img src="images/7.JPG" width="500">

But Failed to connect another device as Network was unreachable 

Then used 
```
ip route
```
But didn't return that routing table or any gateway as network was unreachable 

So,

```
iwconfig
```
* lo = Loopback interface (your own computer)
* eth0 = Wired Ethernet interface
* "no wireless extensions" = eth0 is not a Wi-Fi adapter

<img src="images/8.JPG" width="500">

---

### Checking Network Status
Using Network Manager Command Line Interface to network status. 
```
nmcli device status
```
* nmcli manages/ check network connection in terminal
* device is network device like eth0
* status gives current status of the network device.

<img src="images/9.JPG" width="500">

As you can see, **eth0  ethernet  disconnected** so that, Kali Linux VM can see the network adapter (eth0), but it is not connected to any network.

**Then setting up eth0**

```
ip link set eth0 up
```

* ip Internet Protocol
* link Network link/ interface management
* set Change a configuration
* eth0 Ethernet Interface #0.
* up Administrative state: ON.

<img src="images/10.JPG" width="500">  

Now its On. 

---

### NetworkManager Status 
Firstly checked the NetworkManager is active or unactive. 

```
systemctl status NetworkManager
```

this will give status of Network Manager services 

<img src="images/11.JPG" width="500">  

What it is saying:
* Loaded: loaded (... enabled): This means the system knows what NetworkManager is, and it is set to start up automatically every time you boot up your computer.
* Active: active (running): The service is currently alive and active. It is actively managing your connections right now.
* device (eth0): Activation: starting: NetworkManager noticed you turned eth0 on and is trying to get it fully connected to your network.
* dhcp4 (eth0): activation: beginning: It is currently talking to your internet router to ask for a local IP address (using a system called DHCP) so you can actually browse the web.

Tried to restart it so, 

```
systemclt restart NetworkManager
```

After that, checked the network status again. 
```
nmcli device status
```
<img src="images/12.JPG" width="500">  

What it is saying: 
* Its status is connecting (getting IP configuration): it is currently sitting at the counter waiting for your internet router to hand it an IP address.

 --- 

 ### Tried changing the Adapters

* Settings → Network
* Adapter 1 → Enable Network Adapter
* Attached to: Bridged Adapter or NAT

Then restarted the VM.

<img src="images/13.JPG" width="500">  

---

### Forced the system to drop current network 

Stopped the current connection and rebuild a new connection.
```
nmli connection down "Wired Connection 1
```
Once its Successfully Deactivated, and Reconnect to fresh new connection 
```
nmli connection up "Wired Connection 1"
```
New Connection activated Successfully 

<img src="images/14.JPG" width="500">  

---

### Finally Got Internet Address Configuration on **NAT Adapter**  

<img src="images/15.JPG" width="500"> 

**inet 10.0.2.15/24**: This was the big success! router has officially handed machine a **local IPv4 Address (10.0.2.15)**. officially on the network.

Internet connection is ON and traffic is flowing out to the real world!


**My machine has full, working internet access!**

---
## Providing a Static IP Address

### Checked the Host (MacBook Pro M2) IP Address

First, I checked the IP address of the host machine to identify the network range being used.

```bash
ifconfig en0
```

<img src="images/18.JPG" width="500">

The output showed that the MacBook was assigned the IP address 192.168.0.110 with a subnet mask of 255.255.255.0 (/24).

Since the network range is 192.168.0.0/24, any device connected to the same network can use an IP address such as:
* 192.168.0.1
* 192.168.0.2
* 192.168.0.50
* 192.168.0.110
* 192.168.0.200
* 192.168.0.254

All of these addresses belong to the same network.

**Why 192.168.0.200?**

The IP address 192.168.0.200 was selected as an unused address within the same network.

Example:
Router        = 192.168.0.1
MacBook Pro   = 192.168.0.110
Phone         = 192.168.0.120
Kali Linux VM = 192.168.0.200

This allows the Kali virtual machine to communicate with other devices on the network.

---
### Switched the Network Adapter to Bridged Mode

The virtual machine's network adapter was configured to use Bridged Adapter mode so that it could appear as a separate device on the local network.

After switching to Bridged Adapter mode, a static IP address was assigned manually:
```
sudo ip addr add 192.168.0.200/24 dev eth0
```
This command assigns the static IP address 192.168.0.200 with a subnet mask of 255.255.255.0 to the eth0 network interface.

Next, the default gateway was configured:
```
sudo ip route add default via 192.168.0.1
```
This sets the router (192.168.0.1) as the default gateway, allowing the virtual machine to access external networks and the Internet.

<img src="images/19.JPG" width="500">

---

### Verified Internet Connectivity

Finally, the network configuration was verified by testing Internet connectivity from the Kali Linux virtual machine.

<img src="images/20.JPG" width="500">

The successful response confirmed that the static IP configuration and default gateway settings were correct, and the virtual machine was able to access the Internet successfully.

                                                          ISSUE RESOLVED
