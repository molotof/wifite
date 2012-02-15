wifite
======

Wifite is an automated wireless attack tool.


Requirements
------------

_Wifite is for Linux only._

Wifite must be run as __root__. This is required by the suite of programs it uses.

Wifite was designed for use with [Backtrack 5 R1](http://www.backtrack-linux.org/) Linux distrbution. The script also works on Ubuntu 11/10, Debian 6, and Fedora 16.

Running downloaded scripts as root is a bad idea. I recommend using Backtrack 5 R1 via a bootable Live CD, a bootable USB stick (persistent), or a virtual machine.

Wifite assumes that you have a wireless card and the appropriate drivers that are patched for injection and monitor mode.


Required Programs
-----------------

Please see [the installation guide](https://github.com/derv82/wifite/wiki/Installation) on the wiki for help installing any of the tools below.

* [__Python 2.6.x or 2.7.x__](http://python.org/getit/). Wifite is a Python script and requires Python to run.

* [__aircrack-ng suite__](http://aircrack-ng.org/).
  This is absolutely required.  The specific programs used in the suite are: 
    * airmon-ng, 
    * airodump-ng, 
    * aireplay-ng, 
    * packetforge-ng, and
    * aircrack-ng.

* Standard linux programs.
  * iwconfig, ifconfig, which, iw

Suggested Programs
------------------

_`*` indicates program is not included in [Backtrack 5 R1](http://www.backtrack-linux.org/)_

* `*`[__reaver__](http://code.google.com/p/reaver-wps/), a Wifi-Protected Setup (WPS) attack tool.  Reaver includes a scanner "walsh" (or "wash") for detecting WPS-enabled access points. Wifite uses Reaver to scan for and attack WPS-enabled routers.

* `*`[__pyrit__](http://code.google.com/p/pyrit/), a GPU cracker for WPA PSK keys. Wifite uses pyrit (if found) to detect handshakes. In the future, Wifite may include an option to crack WPA handshakes via pyrit.

* __tshark__. Comes bundled with [Wireshark](http://www.wireshark.org/), packet sniffing software.

* [__cowpatty__](http://www.willhackforsushi.com/Cowpatty.html), a WPA PSK key cracker. Wifite uses cowpatty (if found) to detect handshakes.


