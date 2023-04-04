#### This is a guide for everyone who wants to install fresh Windows 10/11 on their PC.

For this we will need some stuff. Let's get them and get started.

### Requirements:

1. Flash Drive
2. Rufus
3. Windows 10/11 Iso.
4. Internet

### Downloading & Flashing

**1#** We need to download an untouched Windows iso file.

For Windows 10 : https://www.microsoft.com/en-us/software-download/windows10ISO

For Windows 11 : https://www.microsoft.com/software-download/windows11

**2#** Open your desired link in a Chromium Based browser like Chrome/Brave/Edge.

Once the browser loads the page press ctrl+shift+i or simply Right click on a blank space of that page and select Inspect. This will enable inspect mode. Once you see that the page turned into a mobile browser page press the reload button of the browser.

The page will change and you will see option like

**Win10:** Select Edition > Select Language > Downloads > 32/64-bit download.

![](https://i.ibb.co/vqZvpM5/image.png)

**Win11:** Download Windows 11 Disk Image (ISO) for x64 devices > Select Download > Select Language > 64-bit download.

![](https://i.ibb.co/VM5zDns/image.png)

Download and store that iso on a different partition rather than c: drive.

**#3** Now we need to download Rufus. This software is for flashing iso and creating bootable flash drive.

Download the latest version and save it: https://rufus.ie/downloads/

**#4** Now we need to check our HDD/SSD Partition Scheme. Because we don't want any trouble from GPT/MBR. And this is the only important setting that needs to be changed before flashing.

Click Start > Run > type `compmgmt.msc` > click OK, you will see all of your drives showed up.
Then follow this easy tutorial from 1:10 min to get the volume information.
https://youtu.be/3lAYgl_eBlQ?t=70

Now we are ready to flash the iso to the pendrive.

**#5** Connect your pendrive to your pc and run Rufus.
On device, select your pendrive.
On Boot selection, select the Iso we have downloaded before.
On Partition scheme, select MBR or GPT according to your drive volume information.
Then press start and you will get an optional features menu.
This menu depends on the user. You can read and check mark what you need.

![](https://i.ibb.co/pyHpxf0/image.png)

Commonly you can remove Data Collection.

For Win11 requirement bypass you can check mark remove tpm,cpu,ram options.

You can also add user and inputs from here for Win10 and add offline account for Win11.

Press ok and the flashing will start. If Rufus asks that it will format all your data from your pendrive, just say yes.

It will take 8-15 min depending on your flash drive speed.

After finishing, press close.

###  Windows Installation

**6#** Now before we boot into our flash drive we need to get the boot key of your laptop or pc. To do that you can google search by the manufacturer name and add "boot key" example "asus laptop boot menu key" "gigabyte motherboard boot menu key"

This might help : https://www.compressware.in/2022/03/boot-menu-keys-for-all-pc-laptops-motherboard-updated-list.html

Once you get that shutdown your pc connect flash drive then turn on your pc and rapidly press the boot menu key. If you succeed you will see a list of devices that are connected.

Here are some important steps we need to follow in this menu.

On this menu you may see 2 flash drives by the same name but one has a tag like UEFI/EFI.

![](https://i.ibb.co/93xv7qV/image.png)

**If you have a GPT boot drive you need to select the UEFI/EFI flash drive.**

**If you have a MBR boot drive you need to select the usual legacy flash drive.**

If you don't see UEFI/EFI, you are on Legacy BIOS. And probably you have flashed your drive to MBR.

If you don't see UEFI/EFI but your drive is GPT you need to enable UEFI/EFI from your BIOS. You can check the manufacturer Manual for that or you can search your BIOS option one by one.

If you mismatched, just restart and start again.

**#7** Now that you have successfully booted up from your flash drive just read and follow along what windows is telling you once you're on the Custom an Update selection menu select Custom Install.

You will see a list of your drives, if you've done the **#6th** step properly you will not see any EFI/GPT/Legacy/MBR error. You can just select your boot drive then format it then press next to install.

**Beware about formatting. First check for errors then format. Don't rush.**

If you see any error about GPT/MBR just cancel installation and do the **#6th** step properly.

![](https://i.ibb.co/9tC3mS4/image.png)

**#8** If everything goes well the installation will start and finish successfully and ask for restart, you can remove your flash drive now or if you see that the installation starts over again just cancel it, remove the flash drive and restart.

After that it's all about Yes No Yes No stuff. Enter your name/Create an account and get to the Desktop.

**#9** Activating your pc is way easier now. Just follow the massgravel tutorial and Select **HWID** as your activation method.
https://github.com/massgravel/Microsoft-Activation-Scripts

All done. You now have a fresh installation of Windows. Thank you if you read all of it to the end.
I don't have a capturing device but I will add some images in future.
Pardon me for bad English.

Comment if you have more information to share on this topic.

**Notes:**
In some cases, if your drive doesn't show up on the **#7** steps, cancel installation. Normally start your pc and follow this tutorial https://support.hp.com/us-en/document/ish_4859717-4859823-16
