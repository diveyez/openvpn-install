## openvpn-install
OpenVPN [road warrior](http://en.wikipedia.org/wiki/Road_warrior_%28computing%29) installer for Debian, Ubuntu and CentOS.

This script will let you setup your own VPN server in no more than a minute, even if you haven't used OpenVPN before. It has been designed to be as unobtrusive and universal as possible.

### Installation
Run the script and follow the assistant:

`wget https://git.io/vpn -O openvpn-install.sh && bash openvpn-install.sh`

Once it ends, you can run it again to add more users, remove some of them or even completely uninstall OpenVPN.

### Docker Version
Run `docker pull bitnami/minideb`

Run `cd docker && docker-compose up -d`

Now connect to **YOUR HOST IP** on _PORT#_ (*You Chose The Port* _Default: 1194_) 

Using generated <**filename**>**.ovpn** file from **/root/docker/ovpn-files**

Need Permissions? ``chown -R username:groupname /root/docker/ovpn-files/*.ovpn``

Need Quick Automated Setup? 
``docker pull bitnami/minideb && docker exec -it minideb /bin/bash && mkdir /root/docker/open-vpn && cd /root/docker/open-vpn && wget https://git.io/vpn -O openvpn-install.sh && bash openvpn-install.sh`` 
(**Follow On Screen Prompts**) [*Make Sure Port 1194 Is Available If Using That Port*]

### I want to run my own VPN but don't have a server for that

You can get a VPS from just $1/month at [VirMach](https://billing.virmach.com/aff.php?aff=4109&url=billing.virmach.com/cart.php?gid=18).

### Donations

If you want to show your appreciation, you can donate via [PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=VBAYDL34Z7J6L) or [cryptocurrency](https://pastebin.com/raw/M2JJpQpC). Thanks!
