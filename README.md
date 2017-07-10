# TorPhantom
## BETA v0.8
A fork of [TorGhost](https://github.com/susmithHCK/torghost), a little utilitly used to route all traffic through TOR.

Currently depends on macchanger and tor.

This script spoofs your mac address, and then routes all traffic through the TOR network. It is currently a WIP.

## Notice:
Current macOS version does not route ALL traffic through TOR. The current configuration only routes MOST traffic through TOR via socks5 proxy. Any apps not configured to use this proxy (such as a curl call with no proxy flags) will not go through TOR. Proceed with caution!

There is currently no way to fix this, as an equivalent to iptables no longer exists on macOS. Be sure any apps you are using while running TorPhantom are configured to use your proxy settings by default!

If you are aware of another solution to this problem please submit a pull request!

**Remember this tool is still in BETA and any risks you take or activties performed while using TorPhantom fall back on you (whether the app is in BETA or not)**

TODO:
1. Add in arguments for more interfaces other than eth0 and wlan0 on both macOS and Linux (currently hardcoded)
3. More Linux support (currently install script is for Debian based distros only)

DONE:
1. macOS Support


## Linux:
```sh
chmod +x install.sh
./install.sh
```
```sh
  _______         _____  _                 _                  
 |__   __|       |  __ \| |               | |                 
    | | ___  _ __| |__) | |__   __ _ _ __ | |_ ___  _ __ ___  
    | |/ _ \| '__|  ___/| '_ \ / _` | '_ \| __/ _ \| '_ ` _ \
    | | (_) | |  | |    | | | | (_| | | | | || (_) | | | | | |
    |_|\___/|_|  |_|    |_| |_|\__,_|_| |_|\__\___/|_| |_| |_|
	v0.8 - 3ndG4me | www.injecti0n.org

	USAGE:
        torphantom start -----(start torphantom)
        torphantom stop  -----(stop torphantom)
```

## macOS:
#### Install [Mac Ports](https://www.macports.org/install.php)
```sh
chmod +x install.sh
./install.sh
```
```sh
  _______         _____  _                 _                  
 |__   __|       |  __ \| |               | |                 
    | | ___  _ __| |__) | |__   __ _ _ __ | |_ ___  _ __ ___  
    | |/ _ \| '__|  ___/| '_ \ / _` | '_ \| __/ _ \| '_ ` _ \
    | | (_) | |  | |    | | | | (_| | | | | || (_) | | | | | |
    |_|\___/|_|  |_|    |_| |_|\__,_|_| |_|\__\___/|_| |_| |_|
	v0.8 - 3ndG4me | www.injecti0n.org

	USAGE:
        torphantom start -----(start torphantom)
        torphantom stop  -----(stop torphantom)
```
