Quick ADB / Fastboot installer for OS X and Linux (minimal_adb_fastboot)
====================

Last updated: 1.3.2016 | adb version: 1.0.32 Revision eac51f2bb6a8-android
------------------------
Installs the adb and fastboot binaries for OS X and Linux.

If you need the aapt as well, please switch to branch [`aapt`](https://github.com/simmac/minimal_adb_fastboot/tree/aapt) or download the zip [here](https://github.com/simmac/minimal_adb_fastboot/archive/aapt.zip).

Do the following steps:
- Download the zip
- unzip it
- Start the shell script with ./install.sh
- Finished

There are a few arguments you can use with the script:
- uninstall : Deletes the adb and fastboot binaries from /usr/local/bin
	- uninstall-old: For OS X users who installed adb from this script with version <3.0. If you used my script version <3.0 on your mac, you should run this command once to remove the binaries from /usr/bin (they are now installed in /usr/local/bin).
- adb		: Installs the adb binary only
- fastboot	: Installs the fastboot binary only
The arguments can be used like this: ./install.sh [argument] eg *./install.sh uninstall* 
An empty argument does the full installation of both binaries.


Changelog:
---------------
- 1.0	| 15.11.2014 Initial release
- 1.1	| 16.11.2014 Script can now be called from everywhere
- 1.1.1	| 23.11.2014 Name change due to name confict with other adb installer.
- 1.2	| 10.03.2015 Updated adb and fastboot binaries to platform-tools v22, adjusted script because binaries change without version number incremention.
- 1.2.1 | 13.03.2015 Improved version check by adding a hash-check to compare installed and delivered bin. 
- 2.0.0 | 14.03.2015 Added Linux support! (experimental, feedback very welcome!)
- 3.0.0 | 31.05.2015 Improved code quality and readability a lot by rewriting the whole script and using functions. Added the arguments *uninstall*, *adb* and *fastboot*. **Changed the installation path on OS X to /usr/local/bin !**
- 3.1.0 | 05.10.2015 Updated to newest v23 binaries. Required for Android Marshmallow on flounder.
- 3.2.0 | 01.03.2016 Checks if installation directory exists before running the script
- **3.2.1** | 01.03.2016 new branch with aapt-binaries, added aapt-unnstaller


Support Thread:
----------------
Official support thread on xda: http://forum.xda-developers.com/android/general/adb-fastboot-binaries-os-x-inclusive-t2941205
Please open an issue if you experience any problems and feel free to fork and improve this script, I would be happy if you made a push request with your improvements!

This repository is using software from the Android Open Source Project licensed as follows:
'Copyright (c) 2014 Google Inc.

Licensed under the Apache License, Version 2.0 (copy included)'
