# hometransmission
settings for transmission 4 with proxmox lxc ubuntu

Installation steps
1. within Proxmox create a container with latest Ubuntu
2. Update with apt-get or nala
3. Follow the guide for transmission build from their official github and don't forget the dependencies before compiling
4. Change the transmission white list and configure the settings according to your setup
5. If needed change to a third party interface for the web like "flood for transmission", follow the steps accordingly
6. create a symlink with systemd to start transmission automatically at boot/restart
