# Divisé Dark
will update README soon
---------

## W.I.P

Check back soon for a re-write of the README

## Compiling

*I really dont anticipate that anyone will ever attempt to compile this project... but... here goes* ¯\\\_(ツ)_/¯

Requires macOS, and probably a fairly recent version of it. 

Requires `fakeroot`, `ldid`, and `dpkg`. If you dont have them already, they can be easily installed using [homebrew](https://brew.sh):

`brew install fakeroot`

`brew install ldid`

`brew install dpkg`

You may need to edit "succdatroot/Makefile" and change the theos directory from "~/.theos" to "$THEOS" or where ever you have Theos setup. Also edit "compile" and change the IP address to your device's. 

You will need a fairly recent version of theos set up, you can follow their install tutorial [here](https://github.com/theos/theos/wiki/Installation-macOS)

Compiling is fairly simple afterwards, thanks to the `compile` script provided in the root directory of the project. You can use it to compile and install Succession directly onto your device.

***Note**: The install part of the `compile` script will only work if you have OpenSSH installed on your iOS device.*

## License
This project is licensed under the GNU General Public License v3.0, with accordance to [rsync](https://rsync.samba.org/) and [Zebra](https://github.com/wstyres/Zebra). If you'd like to support the project or my development, you can donate [here](https://paypal.me/SamGardner4). **Donations are not a requirement, but highly appreciated!**

Special thanks to [PsychoTea](https://twitter.com/iBSparkes), [Pwn20wnd](https://twitter.com/Pwn20wnd), [Cryptiiic](https://github.com/Cryptiiiic), and [Nobbele](https://github.com/nobbele) for their respective contributions to this project.
