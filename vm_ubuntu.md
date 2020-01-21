$ whoami

# How to Check Ubuntu Version
$ lsb_release -a
Ubuntu 18.04.3 LTS

# apt proxy
https://www.serverlab.ca/tutorials/linux/administration-linux/how-to-set-the-proxy-for-apt-for-ubuntu-18-04/

Acquire::http::Proxy "http://proxy.hostname:8080/";
Acquire::https::Proxy "http://proxy.hostname:8080/";

# wget proxy
$ sudo nano /etc/wgetrc
use_proxy=yes
http_proxy=http://proxy.hostname:8080
https_proxy=http://proxy.hostname:8080


# Install Docker Engine - Community
# Install using the repository
https://docs.docker.com/install/linux/docker-ce/ubuntu/
https://www.digitalocean.com/community/tutorials/como-instalar-y-usar-docker-en-ubuntu-18-04-1-es
https://duo.com/docs/dng#install-docker

#proxy for docker.
https://community.ui.com/questions/Connection-Refused-Failed-to-pull-docker-images/6f817655-56aa-4c3f-83fc-8ff2afd3ac2c

# Failed to connect to download.docker.com port 443
curl -x http://proxy.hostname.es:8080


# For shutdown
sudo poweroff

# For restart
sudo reboot

#
$ netstat -lntp

# docker proxy ubuntu 18.04
