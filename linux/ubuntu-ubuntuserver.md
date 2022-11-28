## issue

1.  When install new ubuntu with setup minimized we can't see suggest pakage like full install.
```
root@ubuntuserver2004:/home/nvth/downloads# java                                                                        
bash: java: command not found  
```
run : 
- `sudo apt-get install command-not-found -y`  
- `sudo reboot`  
- `sudo apt update`  
to fix this!

2.  dpkg: error: dpkg frontend lock is locked by another process  
run :
-  `lsof /var/lib/dpkg/lock-frontend` check `PID`
-  `lsof kill -9 `PID``  
