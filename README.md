## AmneziaVPN (amnezia-client) on Mageia Linux
**Requires:** lib64xcb-util-cursor0 lib64xcb-xinerama0 lib64opengl0

Directories:
```
/usr/local/bin/AmneziaVPN (link)
/opt/AmneziaVPN (work directory)
/opt/AmneziaVPN/client/AmneziaVPN.sh (startup script)
```
Installation from `root`, use from `user`...

1. urpmi --auto lib64xcb-util-cursor0 lib64xcb-xinerama0 lib64opengl0
2. Download [AmneziaVPN_X.X.X.X_Linux_installer.tar.zip](https://github.com/amnezia-vpn/amnezia-client/releases)
3. Unpack and get `AmneziaVPN_Linux_Installer.bin`
4. Installation: su/password `./AmneziaVPN_Linux_Installer.bin`
5. Launch `AmneziaVPN` from the shortcut in the system menu
6. Uninstall (if something is wrong): su/password `./AmneziaVPN_Linux_Installer.bin` 

Connection example [see here...](https://github.com/ImMALWARE/bash-warp-generator)

![](https://github.com/AKotov-dev/AmneziaOnMageia/blob/main/Snapshot1.png) ![](https://github.com/AKotov-dev/AmneziaOnMageia/blob/main/Snapshot2.png)

### Problems?
`AmneziaVPN` actively works with `iptables`. To avoid possible problems, including auto-connection after reboot, you can remove the `shorewall` and `msec` packages: `urpme --auto shorewall-core msec; reboot`, оr disable the `firewall` in the `Mageia control center` in the section `Security` - `Configure personal firewall` (ipv4/ipv6). This decision is up to the user.

`AmneziaVPN` has been tested in MgaRemix-Proserpina - `NetworkManager/nm-applet` & Mageia-9-MATE - `network/net_applet`.

**Useful links:** [Amnezia](https://amnezia.org), [AmneziaVPN](https://github.com/amnezia-vpn), [amnezia-client](https://github.com/amnezia-vpn/amnezia-client)

Many thanks to the creators of the `AmneziaVPN` project.
