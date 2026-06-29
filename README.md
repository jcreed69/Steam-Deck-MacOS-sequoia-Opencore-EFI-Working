# Steam-Deck-MacOS-sequoia-Opencore-EFI-Working
Working EFI for Steam Deck "Deckintosh"

This is a working EFI For Steam Deck LCD and Oled. Currently we have got MacOS Sequoia.

DOESNT WORK/issues:

- Orinatation - always set to portrait and currently trying to find a work around
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
  
   Download the MacRecovery.zip from this repo
  
   Download python (any Version) from the microsoft store or the offical website.
  
   Extract the Zip you downloaded
  
   Whilst in the folder (where you see macrecovery.py) in the search bar of file explorer type "cmd"
  
   Once the terminal opens head to the downloads on this repo and open the MacOS Online Installer cmd Find the version you want and copy the text and paste           as it will download the installer
  
   Once Finished you will see a com.apple.recovery.boot. copy that folder and paste it to your USB

After:

You can edit this Config.plist by using either ProperTree or OCAT

Questions:
   
   - When installing the Local Installer on Windows, you cannot install MacOS Tahoe (26) or MacOS GoldenGate (27 Beta). Here are steps to install Tahoe or GoldenGate
   
        1. install MacOS sequoia Local installer. Follow the steps at Making the Installer(windows) 
       
        2. Boot into the Recovery by installing the EFI from this repo and install the OS
        
        3. Once Setup head to the System update (from MacOS 26 you have to install the updates from the system updates rather than the App store(couldn't find it when looking for the link)
       
        4. Find MacOS Tahoe(if you cant find Goldengate you need to be a developer. follow the steps on Want the Beta versions?) 
       
        5. Once installed the installer, the installer will open up prompting to install follow the instructions. the Mac will restart
    
   - Want the Beta Versions of MacOS (MacOS tahoe (26) and MacOS GoldenGate (27)
        1. On your device go to developer.apple.com and sign in
        2. once done restart system settings or Restart your Mac(recommended)
        3. head back to system update and you will see beta updates. by default it will be Off. Toggle either Public Beta or Developer beta
             - Public beta - MacOS Tahoe (MacOS GoldenGate will be released to Public beta in July 2026)
             - Developer Beta - MacOS Tahoe and MacOS GoldenGate
             - Off - MacOS Tahoe (MacOS GoldenGate will be released to everyone in September 2026)
               
             ---Current Versions---
           
               -Public Beta
                  - MacOS Tahoe - 26.6 Public Beta 2 (build 25G5043d)
                  - MacOS GoldenGate - Not available
                    
               -Developer Beta:
                  - MacOS 26.6 Beta 3 (Build 25G5043d)
                  - MacOS Goldengate 27.0 Beta 2 (Build 26A5368g)
              
               -Off
                - MacOS Sequoia 15.6.1
                - MacOS Tahoe 26.5.2
                - MacOS GoldenGate - Not released to public
      
  
 
    



