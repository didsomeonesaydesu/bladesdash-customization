# bladesdash-customization
### By didsomeonesaydesu
## Tutorial on how to customize the style of Blades dashboard running on Proton/xbGuard

If you've ever used a patched version of the Blades dash on an Xbox 360 stealth server, you may know one of the main downsides is the lack of a working themes setting.
This is an issue, because while you can change your theme background using the regular dashboard, you cannot change the style of the Blades (Carbon and Glass).

Thankfully there is a work around!

## Tools needed:
* Horizon
* Hex editor of your choice

## Instructions

First, copy your Xbox profile to a USB drive if it is not on there already. 

Open Horizon and double your profile from the "Gamer Profiles" folder.

Then, click the "Contents" button and search for the "DashStyle" file in the list. Right click and click extract.

Once, it is extracted, open the file in a hex editor of your choice, I personally use 010Editor, but ImHex is also a good one.

Now, you should see 4 hex digits.
`00 00 00 00`

The last digit should be changed to one of 3 values, (if you have more themes on your profile, there could be more e.g. Halo)


| Theme              | Value |
| ------------------ | ----- |
| Xbox 360 (default) | 00    |
| Carbon             | 01    |
| Glass              | 02    |


For example, if I want to select Carbon:

`00 00 00 01`

Once you have changed the digit, save the file.

Once in Horizon, right click on "DashStyle" again, click replace, and replace the file with your modified "DashStyle".

Now click the red "Save, Rehash, and Resign" button, eject your USB, and plug it back into your Xbox.

Now, when you login, your style should be changed! If you copied your profile to the USB, you are free to copy it back to your HDD.

Enjoy!

