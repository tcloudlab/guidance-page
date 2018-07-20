---
title: about
date: 2017-12-17 02:42:25
---

## Guidance of Using TCloud Networking

#### Network Managers
Currently, the network managers are Jin Zhang and Jiacheng Ma in 5406. The official website manager is Ming Yang in 5408.

#### IP Addressing and DNS
The lab use DHCP assign IP addresses. When connected to the lab's network, your device will be assigned an IP from range 10.0.1/21 if you are inside the lab, or from range 10.0.8/21 if you are connected via VPN. **Your DNS hostname will be added to the DNS automatically.** TCloud Network has a default domain <u>tcloud.moe</u>, which means if the hostname of your device is <u>alice</u>, the domain auto-assigned will be <u>alice.tcloud.moe</u>. The domain assigned can only be resolved and accessed inside the lab. **Please use a hostname you can remember, and don't use too simple hostname to avoid conflict.**

#### Important IP Addresses, Domains, and Links
TCloud's Public IP Address: <u>202.120.40.100</u>
DNS Server: <u>10.0.0.254</u> <u>dns.tcloud.moe</u>
Printer in 5406: <u>10.0.2.125</u> <u>printer-5406.tcloud.moe</u> <u>printer-5406</u>
Printer in 5404: <u>10.0.3.176</u> <u>printer-5404.tcloud.moe</u> <u>printer-5404</u>
Public Proxy (HTTP Proxy, Account Needed): <u>202.120.32.250:5678</u>
Cloud Storage: <u>file.tcloud.moe</u>
Private Proxy (PAC Proxy, In-Lab Only): <u>pac.tcloud.moe</u>
Private Proxy (HTTP Proxy, In-Lab Only): <u>proxy.tcloud.moe</u>
VPN Password Manager: <u>usermin.tcloud.moe</u> <u>usermin</u>
This Page: <u>net.tcloud.moe</u> <u>net</u>

#### Port Forwarding
Based on some security consideration, **only servers are allowed to expose ports on the internet**. (We found that our public ports are scanned very often.) Otherwise please use the VPN. Contact the network managers for more information.

#### Cloud Storage
The cloud storage system is based on seafile, and only accessible when connected to the lab network (inside the lab or via VPN). The URL is [http://file.tcloud.moe](http://file.tcloud.moe) or [http://file](http://file). Contact one of the network managers to get an account.

#### Chatting Room
The chatting room locates in http://chat.tcloud.moe. No account is needed. Contact one of the network manager to add a channel.

#### VPN
The lab offers VPN to access the workstations, servers, and other services inside the lab (5402`~`5408). Our VPN uses the open source SSL VPN server *ocserv*, and are compatible to the Cisco AnyConnect. You can use *OpenConnect* or *Cisco AnyConnect* to connect.

**The VPN can be only used for academic purpose**, such as using the lab services from outside the lab, connecting to a service inside the lab, communicating with colleagues in the in-lab chatting room, etc. User of the VPN are not allowed to share the account, send the account password to others, or abuse the service in any way.

**Please contact one of the network managers for a VPN account.** They will give you an account with a default password, and you can change the password later in http://usermin.tcloud.moe (only accessible inside the lab).

Install one of the VPN software listed below, then use <u>202.120.40.100</u> to connect. While first connecting, you may need to ignore the Certification warning.

###### VPN Software
* Cisco AnyConnect: [Windows](vpn/anyconnect-win-4.5.04029-core-vpn-predeploy-k9.msi) | [MacOS](vpn/anyconnect-macos-4.5.04029-predeploy-k9.dmg) | [Linux](vpn/anyconnect-linux64-4.5.04029-predeploy-k9.tar.gz)
* OpenConnect GUI: [Windows and MacOS](https://github.com/openconnect/openconnect-gui/releases)
* OpenConnect: [GitHub](https://github.com/openconnect/openconnect) (Linux users may install it via package control tools.)
* NetworkManager: You may install [this](network-manager-openconnect-gnome) package or find more information [here](http://www.infradead.org/openconnect/gui.html).
* IOS and Android: Download it from the official app store.

#### Proxy
When you are inside the lab (5402`~`5408) or connected via the VPN, you can use this PAC file: <u>pac.tcloud.moe</u>, or this HTTP proxy: <u>proxy.tcloud.moe:5678</u>. (This pac is only accessible inside the lab.) Otherwise, please use this HTTP proxy address: <u>202.120.32.250:5678</u>. **For Windows machines inside the lab, the proxy is auto-configured.**

#### Moe
A place to publish black history of the lab. Hosted on GitHub: [https://tcloud.moe](https://tcloud.moe). Join the GitHub Oragination [tcloudlab](https://github.com/tcloudlab) to add something on it.
