---
title: "OpenVPN"
---

We'll use OpenVPN install script.

# Downloading Script

```
curl -O https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
```

# Running Script

```
sudo ./openvpn-install.sh
```

For IP address, just press enter.

If you wanna use IPV6, you can say `y`, if you don't want, you can say `n`.

In port choice, I recommend using Random.

In Protocol, I recommend UDP. If it's not available, just use TCP.

Select a DNS to use in your VPN. I recommend Adguard DNS.

In compression, I recommend `n`.

In encryption settings, I recommend `n`. Because script is setting a lot of settings already. We don't need to modify them.

Script will install packages.

We'll create a client. It can be your PC, phone etc. Give a name for it.

If you wanna use a password, you can select it.

It will create ovpn file in your home directory. We need to download this file to your host machine.

You can use sftp in your host machine.

# Connecting

Download OpenVPN, and connect to your VPN.

If you are using KDE Plasma, you don't need to download OpenVPN app. Just go to
* Settings
* Wi-Fi & Internet
* `+`
* Import new connection
* Select your OVPN file
* Click to network button in your taskbar
* Find your VPN connection
* Click Connect
