# hometransmission
Build and setup for transmission 4 with proxmox lxc ubuntu

https://youtu.be/N-RXqnlAqf0

All files shared here are based on the setup shown in the video. File permissions need to be set if you are using anything other than root.

Installation steps
1. Within Proxmox create a container with latest Ubuntu
2. Update with apt-get or nala
3. Follow the guide for transmission build from their official github and don't forget the dependencies before compiling
4. Change the transmission white list and configure the settings according to your setup
5. If needed change to a third party interface for the web like "flood for transmission", follow the steps accordingly
6. Create a symlink with systemd to start transmission automatically at boot/restart. Point to note under system the type should be simple:
[Service]
Type=simple
7. Setup Samba and apply the settings according to your environment. New Samba doesn't require for a linux user. You can create within a separate samba user.
