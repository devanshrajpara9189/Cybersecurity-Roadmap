# Troubleshooting Internet Connection Issue
I was having trouble getting an internet connection in VirtualBox on my M2 Mac, even though my host system was connected to Wi-Fi. I tried using a Bridged Adapter, but **DHCP completely failed** to assign an IP address. After trying various fixes, I finally resolved it by manually configuring a **static IP** inside the VM.

### 📸 Here, I have attached all the screenshots showing the issues I encountered and the steps I followed to successfully resolve them.
I received valuable guidance and support from my professional instructor.
### Firstly:
I checked the ip address 
```
ip a
```

<img src="images/1.png" width="500">

**There was a corrupted Zsh history file, which I fixed by clearing the history and restarting the terminal session** 


<img src="images/2.JPG" width="500">

For resloving the issue there are few commands. 
```
mv ~/.zsh_history ~/.zsh_history.bak
```
* mv = move or rename a file.
* ~/.zsh_history = your current Zsh history file.
* ~/.zsh_history.bak = backup file.
```
touch ~/.zsh_history
```
* touch: creates a new empty file if it doesn't exist.
```
chmod 600 ~/.zsh_history
```
* chmod changes file permissions.
* 600 means:
     * Owner: Read + Write (rw-)
     * Group: No permissions (---)
     * Others: No permissions (---)

 ```
exec zsh
```
* exec replaces the current shell process with a new one
* zsh starts a fresh Zsh session.
    
<img src="images/3.JPG" width="500">

