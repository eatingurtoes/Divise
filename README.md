# SuccessionDown

---------

## Tethered Downgrades

Either download a deb from the releases tab or add my [repo](matthewpierson.github.io) and install it from there

This fork is purely for tethered downgrades! This is likely very unstable, probably won't work and might damage your device. It will probably be fine but be warned. 

To perform a tethered downgrade using this, simply open the app, click "Download clean filesystem", enter what iOS version you wish to downgrade to and let it do it's stuff!

You are still restricted by SEP compatibility, which the app will check after you input an iOS version. The app will also not let non-checkm8 devices nuke their iOS install by running this.

Apple is still blocking older IPSW downloads, seemingly at random, so if you are unable to download one iOS version either try again, wait a few hours and try again or pick a different iOS version. 

DO NOT, I repeat, DO NOT annoy/message/spam/question Samg_is_a_Ninja about any issues that occur with this fork, please direct all of them to me as I don't want him to have to deal with the various issues this fork will likely have. Either on [twitter](https://twitter.com/mosk_i) or here on GitHub.

-------------

Alternative to Cydia Eraser that is much easier to update. Downloads and mounts rootfilesystem DMG for your iOS version. Then moves files from mounted DMG to the main filesystem.

Special thanks to @pwn20wndstuff, @PsychoTea, @Cryptiiic, @4ppleCracker for their respective contributions to this project.

This project is free (and always will be), donations are never required but highly appreciated: https://paypal.me/SamGardner4

*rsync used in accordance with gpl3*

*attach generously provided by comex*

## Device Support

A8(x) and A9(x) support will come when checkm8 supports them

- iPhone 5s
- iPhone 7/7 Plus
- iPhone 8/8 Plus
- iPhone X

- iPad 6th Gen
- iPad 7th Gen
- iPad Mini 2/3
- iPad Air
- iPad Pro (Whichever ones are A10(x)/A11(x) should work fine c: )

- iPod 7th Gen

If you want a full list/more details, download [this plist](http://matthewpierson.github.io/sep.plist) and look through it!

## Compiling

*I really dont anticipate that anyone will ever attempt to compile this project... but... here goes* ¯\\\_(ツ)_/¯

Requires macOS, and probably a fairly recent version of it. 

Requires `fakeroot`, `ldid`, and `dpkg`. If you dont have them already, they can be easily installed using [homebrew](https://brew.sh):

`brew install fakeroot`

`brew install ldid`

`brew install dpkg`

You may need to edit "succdatroot/Makefile" and change the theos directory from "~/.theos" to "$THEOS" or where ever you have Theos setup. Also edit "compile" and change the IP address to your device's. 

Once you have the dependencies, compiling is fairly easy, just run the compile script in the root directory of this project, it will automatically create a .deb file for installation. You can also use the "install" script to automate the installation process, this requires OpenSSH or dropbear or some alternative of it and SFTP to be available on your device (OpenSSH has both). The install script used to be a part of the compile script, but I got annoyed by it so I split the two. I might delete the install script some day, idk.
