# CodeSpace-VM

# The commands I ran
```docker run --privileged --shm-size 1g -d -p 8080:10000 -e VNC_PASSWD=password -e PORT=10000 -e AUDIO_PORT=1699 -e WEBSOCKIFY_PORT=6900 -e VNC_PORT=5900 -e SCREEN_WIDTH=1024 -e SCREEN_HEIGHT=768 -e SCREEN_DEPTH=24 thuonghai2711/ubuntu-novnc-pulseaudio:20.04```

The password is literally password, make sure to make the ports public PLEASEEEEEEEEEEE 
also yes this is novnc with audio somehow

Also, with novnc it sometimes disconnects you. This can be AVOIDED with the simple advanced feature, autoreconnect! Make the reconnect delay about ~1000ms.

To stop the server, type `docker ps` to see the name, then type `docker stop <name>`, where `<name>` is the name of the running container.
Type `docker rm <name>` to remove it ENTIRELY. Very good for hiding what you do online. 

> |-| NOTE: THIS WILL DELETE YOUR FILES. |-|

---
# How it works:
Docker is pre installed on every codespace and gitpod instance, so we can use this to make a virtual machine running docker and novnc with audio!