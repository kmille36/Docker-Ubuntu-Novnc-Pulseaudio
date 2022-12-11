# Docker-Ubuntu-Novnc-Pulseaudio
Concept Of Ubuntu VNC with noVNC + Pulse Audio Server Running.  

![image](https://user-images.githubusercontent.com/58414694/206900314-e30d5f8b-ef59-4b86-9c38-cf8fb7045319.png)

Paste this in Google Cloud Shell Terminal, then preview on port 8080 for noVNC, User/Pass: password: password

- Ubuntu 20.04:

 ```console  
docker run --privileged --shm-size 1g -d -p 8080:10000 -e VNC_PASSWD=password -e PORT=10000 -e AUDIO_PORT=1699 -e WEBSOCKIFY_PORT=6900 -e VNC_PORT=5900 -e SCREEN_WIDTH=1024 -e SCREEN_HEIGHT=768 -e SCREEN_DEPTH=24 thuonghai2711/ubuntu-novnc-pulseaudio:20.04
```

- Ubuntu 22.04:

 ```console  
docker run --privileged --shm-size 1g -d -p 8080:10000 -e VNC_PASSWD=password -e PORT=10000 -e AUDIO_PORT=1699 -e WEBSOCKIFY_PORT=6900 -e VNC_PORT=5900 -e SCREEN_WIDTH=1024 -e SCREEN_HEIGHT=768 -e SCREEN_DEPTH=24 thuonghai2711/ubuntu-novnc-pulseaudio:22.04
```
