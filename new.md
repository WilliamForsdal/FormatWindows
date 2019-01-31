## Prepare
Before reinstalling windows the following should be considered:

1. Drivers and other software
   
   Download all drivers and software needed before reinstalling windows. This makes the process afterward easier.
   * [Ninite](https://ninite.com/)
   * [Speedcrunch](http://www.speedcrunch.org/)
   * [ConEmu - better windows terminal](https://conemu.github.io/)
   * [Flux](https://justgetflux.com/)
  
2. Windows activation

   How will windows be activated? Know this before reinstalling.
  
3. Media creation tool

   Use the Media creation tool [from here](https://www.microsoft.com/sv-se/software-download/windows10) to put the windows installer on a 8GB USB disk.
  
4. Disconnect hard drives

   Disconnect all hard drives except the one that windows will be installed on. This eliminates the risk of formatting the wrong hard drive, and also makes it impossible for the windows installer to install files on other disks during the setup.
  
## Install windows
When the preparation is finished install windows on the selected hard drive.

## Install software
Install the software you want to have installed.

## Tweaks

* Download [Windows Tweaker](https://www.thewindowsclub.com/ultimate-windows-tweaker-4-windows-10)

  Great tool for changing many settings in windows.

  
* Turn off skype ads

  Open the start menu and search for "Internet Options" * go to security, click restricted sites and then sites, block g.msn.com and apps.skype.com

  
* Turn off hotkey for sticky keys
   
  press shift x5 and turn off sticky keys
   
   
* Show file extensions and other explorer stuff
   
  Open File Explorer and in the upper left corner, select file -> Change folder and search options, and select the general tab.
  
  * Set standard startup folder to This PC. 
  
  * Disable folder history.
  
  * Switch to the View tab and untick "hide extensions for known file types".
   
   
* Add programs to run at windows startup

  Adding shortcuts to this path: C:\Users\ \<Username\> \AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup
  
  makes them run on startup.
  
  
* Set correct locale
  
  Go to: Control Panel -> Region -> Administrative -> Change system locale
  
  And select the correct one.
  
  
* Disable ctrl+shift hotkey that changes input language

  The most annoying hotkey in windows. How do you remove this in latest windows?
  

* Change power options
  
  Go to Control Panel -> Hardware and Sound -> Power Options. Select High Performance.
  
  Also click "Change plan settings" to the right, and customize the settings in there. 
  
  
* Disable waking from magic packets

  If your computer is waking up randomly from hibernation/sleep, it is probably due to this.
  
  To turn this off, right click the start menu and select Device Manager. Under network adapters, right click your ethernet adapter
  
  and select properties. Under the power management tab, under Wake on LAN, untick "Wake on magic packets".
  
  
* Turn off hibernation to save SSD space

  Do this if you have a small SSD and dont use hibernation.
  
  Start CMD as admin and write "powercfg -h off" without the quotes. This removes the large hiberfil.sys file from the drive.
  

* Changing page file size

  *WARNING* do not do this unless your SSD is really small and you need the extra space. Windows uses the pagefile for virtual memory.
  
  Open the start menu and search for "Adjust the appearance and performance of Windows". Switch to the Advanced tab and change the virtual memory size.
  

* Turn off useless windows features

  In the Control Panel, Go to programs and features, and select "Turn windows features on or off" on the left side.
  
  Untick Internet Explorer, Media Features, Games.
  
  
* Stop windows from creating system images automatically

  Go to Control Panel -> Recovery and select the "System Protection" tab. Press the Configure button and Disable system protection.
  
  
* Change computer name
  
  Right click this PC (in the left side of the explorer) and select Properties. 
  
  Under "Computer name, domain, and workgroup settings, click "Change settings" (on the right side) and select the "Computer name" tab, and click change on the bottom.
  
  


  
  

  
  
  
  

  
  
  







