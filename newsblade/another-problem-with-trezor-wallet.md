---
title: Another problem with Trezor wallet
date: 2017-09-12 10:35:41 +0000
datetime: 2017-09-12 00:00:00 +0200
---


From [Reddit](https://www.reddit.com/r/Bitcoin/comments/6zgocf/psa_trezor_privacy_leak_trezor_windows_driver/):

The Trezor Bridge Windows installer puts a link to the driver trezord.exe into autostart to have it launched with every system start. One of the first things this executable does is download two files from wallet.trezor.io (hosted on Amazon servers).

Source: https://github.com/trezor/trezord/blob/master/src/main.cpp

How could one make it easier for governments to track Bitcoin users and put them at risk of the driver being shut down remotely? This is nuts!

Please complain to the guys at Trezor to have them improve this driver and crank up their sensitivity for privacy! Being the first hardware wallet this device really deserves better.

A short term solution would be to remove the driver and only use Electrum instead of web wallets. Note that for me this driver does not show up under installed programms so I had to use the explorer to manually launch the uninstall program by starting c:\program files (x86)\TREZOR Bridge\Uninstall.exe

Continued from: https://np.reddit.com/r/TREZOR/comments/6yti7p/trezor_bridge_trezordexe_calling_home/

edit: From the code it looks like Linux and Mac versions show the same behaviour on execution, not sure about whether they are automatically installed to be run at system start (I guess not).

edit2: It seems some people don't see what upsets me so much about programms calling home. Imagine a government would like to keep track of all Bitcoin users. Just in case they would like to confiscate or make Bitcoin illegal at some point of time in the future. Bad practice like this makes it a lot easier for them.