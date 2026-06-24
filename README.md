# Steam-Deck-MacOS-sequoia-Opencore-EFI-Working
Working EFI for Steam Deck

This is a working EFI For Steam Deck LCD and Oled. Currently we have got MacOS Sequoia.

DOESNT WORK/issues:

- Orinatation always set to portrait and currently trying to find a work around
- Wi-Fi and Bluetooth - unless changed to an intel chip or by buying a Wi-Fi adaptor
- Screen brightness - unless connected to external display or screen mirroring
- Airdrop and Location services - all of these needs Wi-Fi and bluetooth 
- Touchscreen
- sound

Works: 

- MacOS Sequoia or other past Versions
- Screen mirror
- Trackpad - Both Work
- Connecting a USB hub
- 4MB of Graphics - thats what i have
- USB Tethering - can be used to get network
- Apple ID / Messages / Facetime and other services
- Dual Booting steamOS, Windows 11 and MacOS 

What you need:

- EFI downloaded from this project
- USB Drive 32GB+
- Windows or Mac
- Make sure you correctly partition your Hard drive especially if you want to dual-boot

Instructions

- Download the EFI if you havent yet from this repo

- Format your USB Drive to Fat32 by using on DiskUtil(macOS) / Rufus(windows / Disk Managment (windows)

  Making the installer(MacOS)
  - On the App store download the OS you want to install (Certain Mac devices cannot install the MacOS you want if the device can support it)
  - Once Downloaded Head to Finder > Applications and right click the Installer and select "Show Package Contents"
  - once inside the installer head to Contents > Resources and right click the file which has the name CreateInstallMedia and copy the file
  - Once done open the terminal app and enter sudo (paste what you just copied) --volume /Volumes/(your USB name)
  - Once entered enter your sudo password and select Y and it will start downloading to your USB.
 
  Making the installer(windows)

  Before you continue

  - you will need to download the MacRecovery.Zip from this repo
  - The installer you make is the Online installer. Requires USB tethering - Kext Loaded in EFi
 
   Steps:
       - Download the MacRecovery.zip from this repo
       - Download python (any Version) from the microsoft store or the offical website.
       - Extract the Zip you downloaded
       - Whilst in the folder (where you see macrecovery.py) in the search bar of file explorer type "cmd"
       -Once the terminal opens head to the downloads on this repo and open the MacOS Online Installer cmd Find the version you want and copy the text and paste           as it will download the installer
       -Once Finished you will see a com.apple.recovery.boot. copy that folder and paste it to your USB
  
 
    



