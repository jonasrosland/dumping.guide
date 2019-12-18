---
title: "3DS"
date: 2019-12-17T20:07:03-05:00
draft: false
weight: 1
---

### Nintendo 3DS GodMode9 Method

**Temporarily running GodMode9**

If you do not wish to hack your 3DS, but still own a [compatible flashcart][1], you can simply install ntrboot onto the cart, and download GodMode9, renaming the _GodMode9_ntr.firm_ file from the ntrboot folder in the GodMode9 download. After that, perform ntrboothax (see the guide!) and skip to Dumping.

**Tools**
* A Nintendo (New) {2/3}DS with a method to run "bare-metal" ARM9 software. Methods include having a [custom firmware][2] installed or a DS flashcart with ntrboothax.
* [GodMode9][3] (Ensure you are using the latest so you can notate the gamecart ID.)

**Dumping**

* Run GodMode9
* Copy down the ID in brackets to the side of GAMECART (if it's not there, navigate into GAMECART then return back to the main menu)
* Navigate into "GAMECART"
* Copy the .3ds file without trim in its name to the SD card. If split files show up (for 3DS games that are >=4GB), you will need to copy those.
* If you copied the ROM in split form, you need to combine them using copy /b part1 + part2 combined on the Windows command line or cat part1 part1 > combined on the Mac OS or Linux terminal. Otherwise, you're done.

---

### Gathering Dump Info
* Dumping Tool: The name and version of the tool/method use to make the dump.
* CRC32: Generated from the ROM file using HxD, for example.
* MD5: Ditto.
* SHA-1: Ditto.
* Game title: If it differs between different places (e.g. title screen, console menu banner, box, cart) then go with the one on the front of the box.
* Region: The region the disc originated from like USA, Japan or Europe
* ROM Revision: The revision found in the ROM data.
* ROM Serial: The 10-character serial found at 0x1150 the ROM data, in the format "XXX-X-XXXX" with X being a letter or number.
* Languages/Language Select: Some games either show a language selection screen at startup or in the game options. Many games will boot with different * languages depending on the active language selected in the BIOS. Booting the game with each language selected in the bios is necessary to identify the * supported languages for these games. Note that it is possible to submit a game without checking the languages, but this then needs to be stated in your * submission.
* Tip: Using an emulator like Citra can speed up the language checking dramatically since you can switch the system language in the emulator settings much faster than on a real 3DS.
* Cart Serial: It is located on the label on the front of the cart the form of "LNA-CTR-AREP-EUR" (where X is a letter or number), also it may have a number * (Like -1 or -2) appended.
* Cart Additional Serial: On back of cart.
* Box Barcode: The number on the case displayed beneath the vertical lines, see Barcode.
* Box Serials: The serials on the case. Example: CTR P AREP, TSA-CTR-AREP-UKV, Art.-Nr.:2221246T
* Size: The size of the ROM in bytes.
* Chip(s) serial(s) (optional): The codes on the ROM chip inside the cart. You would need to break open the cart to see these.
* Scans: The following scans (or photos) would be good to have: Front and back of the following items - box, cart and PCB.


**Submitting Info to No-Intro**
If you have datter rights you can submit the dumpinfo using the "Submit" form in DAT-o-MATIC.

Otherwise post the info in the New Dumps & Redumps section of the forum.

[1]: https://3ds.hacks.guide/ntrboot
[2]: https://3ds.hacks.guide/
[3]: https://github.com/d0k3/GodMode9/releases/latest