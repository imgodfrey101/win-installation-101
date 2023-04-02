<span class="bbcode-size-14"><b>This is a guide for everyone who wants to install fresh Windows 10/11 on their PC.</b></span><br>
<br>
For this we will need some stuff. Let's get them and get started.<br>
<br>
<span style="color:#59e817">Requirements:<br>
1#Flash Drive<br>
2#Rufus<br>
3#Windows 10/11 Iso.<br>
4#Internet </span><br>
<br>
<span style="color:#cddc39">Downloading & Flashing</span><br>
<br>
<span style="color:#ff8040">1#</span> We need to download an untouched Windows iso file.<br>
<br>
For Windows 10 : https://www.microsoft.com/en-us/software-download/windows10ISO<br>
<br>
For Windows 11 : https://www.microsoft.com/software-download/windows11<br>
<br>
<span style="color:#ff8040">2#</span> Open your desired link in a Chromium Based browser like Chrome/Brave/Edge.<br>
<br>
Once the browser loads the page press ctrl+shift+i or simply Right click on a blank space of that page and select Inspect. This will enable inspect mode. Once you see that the page turned into a mobile browser page press the reload button of the browser.<br>
<br>
The page will change and you will see option like<br>
<br>
Win10: Select Edition &gt; Select Language &gt; Downloads &gt; 32/64-bit download.<br>
<br>
<a href="https://ibb.co/02hVTzN"><img src="https://i.ibb.co/vqZvpM5/image.png" /></a><br>
<br>
Win11: Download Windows 11 Disk Image (ISO) for x64 devices &gt; Select Download &gt; Select Language &gt; 64-bit download.<br>
<br>
<a href="https://ibb.co/zPDBb9z"><img src="https://i.ibb.co/VM5zDns/image.png" /></a><br>
<br>
Download and store that iso on a different partition rather than c: drive.<br>
<br>
<span style="color:#ff8040">#3</span> Now we need to download Rufus. This software is for flashing iso and creating bootable flash drive.<br>
<br>
Download the latest version and save it: https://rufus.ie/downloads/<br>
<br>
<span style="color:#ff8040">#4</span> Now we need to check our HDD/SSD Partition Scheme. Because we don't want any trouble from GPT/MBR. And this is the only important setting that needs to be changed before flashing.<br>
<br>
Click Start &gt; Run &gt; type compmgmt.msc &gt; click OK, you will see all of your drives showed up.<br>
Then follow this easy tutorial from 1:10 min to get the volume information.<br>
https://youtu.be/3lAYgl_eBlQ?t=70<br>
<br>
Now we are ready to flash the iso to the pendrive.<br>
<br>
<span style="color:#ff8040">#5</span> Connect your pendrive to your pc and run Rufus.<br>
On device, select your pendrive.<br>
On Boot selection, select the Iso we have downloaded before.<br>
On Partition scheme, select MBR or GPT according to your drive volume information.<br>
Then press start and you will get an optional features menu.<br>
This menu depends on the user. You can read and check mark what you need.<br>
<br>
<a href="https://ibb.co/fv372k1"><img src="https://i.ibb.co/pyHpxf0/image.png" /></a><br>
<br>
Commonly you can remove Data Collection.<br>
<br>
For Win11 requirement bypass you can check mark remove tpm,cpu,ram options.<br>
<br>
You can also add user and inputs from here for Win10 and add offline account for Win11.<br>
<br>
Press ok and the flashing will start. If Rufus asks that it will format all your data from your pendrive, just say yes.<br>
<br>
It will take 8-15 min depending on your flash drive speed.<br>
<br>
After finishing, press close.<br>
<br>
<span style="color:#cddc39">Windows Installation </span><br>
<br>
<span style="color:#ff8040">6#</span> Now before we boot into our flash drive we need to get the boot key of your laptop or pc. To do that you can google search by the manufacturer name and add "boot key" example "asus laptop boot menu key" "gigabyte motherboard boot menu key" <br>
<br>
This might help : https://www.compressware.in/2022/03/boot-menu-keys-for-all-pc-laptops-motherboard-updated-list.html<br>
 <br>
Once you get that shutdown your pc connect  flash drive then turn on your pc and rapidly press the boot menu key. If you succeed you will see a list of devices that are connected.<br>
<br>
Here are some important steps we need to follow in this menu.<br>
<br>
On this menu you may see 2 flash drives by the same name but one has a tag like UEFI/EFI.<br>
<br>
<a href="https://ibb.co/zH35zS7"><img src="https://i.ibb.co/93xv7qV/image.png" /></a><br>
<br>
If you have a GPT boot drive you need to select the UEFI/EFI flash drive.<br>
<br>
If you have a MBR boot drive you need to select the usual legacy flash drive.<br>
<br>
If you don't see UEFI/EFI, you are on Legacy BIOS. And probably you have flashed your drive to MBR.<br>
<br>
If you don't see UEFI/EFI but your drive is GPT you need to enable UEFI/EFI from your BIOS. You can check the manufacturer Manual for that or you can search your BIOS option one by one.<br>
<br>
If you mismatched, just restart and start again.<br>
<br>
<span style="color:#ff8040">#7</span> Now that you have successfully booted up from your flash drive just read and follow along what windows is telling you once you're on the Custom an Update selection menu select Custom Install.<br>
<br>
You will see a list of your drives, if you've done the #6 step properly you will not see any EFI/GPT/Legacy/MBR error. You can just select your boot drive then format it then press next to install.<br>
<br>
Beware about formatting. First check for errors then format. Don't rush. <br>
<br>
If you see any error about GPT/MBR just cancel installation and do the #6th step properly.<br>
<br>
<a href="https://ibb.co/4d5gw3S"><img src="https://i.ibb.co/9tC3mS4/image.png" /></a><br>
<br>
<span style="color:#ff8040">#8</span> If everything goes well the installation will start and finish successfully and ask for restart, you can remove your flash drive now or if you see that the installation starts over again just cancel it, remove the flash drive and restart.<br>
<br>
After that it's all about Yes No Yes No stuff. Enter your name/Create an account and get to the Desktop.<br>
<br>
<span style="color:#ff8040">#9</span> Activating your pc is way easier now. Just follow the massgravel tutorial and Select HWID as your activation method.<br>
https://github.com/massgravel/Microsoft-Activation-Scripts<br>
<br>
All done. You now have a fresh installation of Windows. Thank you if you read all of it to the end. <br>
I don't have a capturing device but I will add some images in future.<br>
Pardon me for bad English.<br>
<br>
 Comment if you have more information to share on this topic.<br>
<br>
<span style="color:#59e817"><b>Notes</b></span><br>
#In some cases, if your drive doesn't show up on the #7 steps, cancel installation. Normally start your pc and follow this tutorial https://support.hp.com/us-en/document/ish_4859717-4859823-16
