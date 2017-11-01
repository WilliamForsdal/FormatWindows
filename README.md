1. Install windows
    * If the pc has more than one physical hard disk/drive installed, it could
    happen that windows installs things on other drives than the selected C drive. To 
    be sure, disconnect ALL drives except the selected C drive.
    
2. Install drivers (windows 10 helps with this)
    Its best to download drivers before formatting and re-installing windows.

4. Download and Install Ninite. Ninite is an all in one installer for commonly used software.
	* go to ninite, check all the programs you want, click download and install.
    * Recommended:
        - WinDirStat: gives a nice overview of all files on your hard drives.
        - GreenShot: used to take snapshots of the desktop.
        - Paint.NET: better than normal windows MS Paint / Paint 3D (ew)
        - LibreOffice: good alternative for Microsoft Office
        - Notepad++: better than normal windows notepad.
        - 7-Zip: better zip than WinRAR

----------------------------------------------
5. Windows settings:

Remove ALL windows default "apps" 
WARNING This will remove all the xbox, candy crush bullshit (but also the standard photo viewer app AND CALCULATOR)
    * Open the start menu, type "PowerShell" and run as administrator
    * Paste the following (without the qoutes): "Get-AppXPackages | Remove-AppXPackage"
    * See this video https://youtu.be/5x2VTN4jjIE?t=374
    * (A good replacement if the calculator is removed is http://www.speedcrunch.org/ )

Increase privacy:
    * Download Ultimate Windows Tweaker http://www.thewindowsclub.com/ultimate-windows-tweaker-4-windows-10
        Go to Security & Privacy and go to the Privacy tab and disable everything.
        Look through the other menus and tweak other things if you want.

    * Download Spybot Anti-Beacon https://www.safer-networking.org/spybot-anti-beacon/
        If you do not use OneDrive you can disable everything.
        
Turn off skype ads:
	* Open the start menu and search for "Internet Options"
	* go to security, click restricted sites and then sites, block g.msn.com and apps.skype.com

Turn off hotkey for sticky keys
	* press shift x5 and turn off sticky keys

Remove OneDrive COMPLETELY (https://www.windowscentral.com/how-remove-onedrive-file-explorer-windows-10)
WARNING don't trust strangers telling you to paste things into CMD, do this at your own risk
	* start CMD as administrator
		* FOR 64BIT WINDOWS: paste "%SystemRoot%\SysWOW64\OneDriveSetup.exe /uninstall" (WITHOUT THE QUOTES) and press enter (if you dare)
		* FOR 32BIT WINDOWS: paste "%SystemRoot%\System32\OneDriveSetup.exe /uninstall" (WITHOUT THE QUOTES)  and press enter (if you dare)
	* open regedit (win+r and type regedit and hit enter)
	* Navigate to the HKEY_CLASSES_ROOT\CLSID\{018D5C66-4533-4307-9B53-224DE2ED1FE6} key
	* open System.IsPinnedToNameSpaceTree and change it from 1 to 0.

Language for non unicode programs
	* Go to Control Panel\Region\Administrative
	* Change system locale to your language.
	* Go to tab Location and change Home location to your country.

disable ctrl+shift hotkey that changes input language
	* Open Control Panel, go to "Clock, Language and Region" -> "Language" -> "Advanced Settings"
	* click "Change language bar hot keys".
	* Under the Advanced Key Settings tab, under "Hot keys for input languages", remove all hotkeys.
	
Folder options
	* Open File Explorer and in the upper left corner, select file -> Change folder and search options
	* Set standard startup folder to This PC
	* Disable folder history
	* disable hide extensions for known file types

Energy options
	* Go to Control Panel\Hardware and Sound\Power Options
	* Check High Performance
	* Change plan settings for High performance
	* Change advanced power settings
	* Change sleep, hiberntion and hybrid sleep to what you want
	
Disable waking from "magic packets"
	* Open start menu, search for "Device Manager" and click enter
	* Under network adapters, right click your ethernet adapter and select properties
	* Under the Power Management tab, under Wake on LAN:, deselect "Wake on Magic Packet"
	
If you don't want hibernation (for users with smaller SSDs this will free up some space)
	* Start CMD as admin
	* write "powercfg -h off" without the qoutes
	(this removes the hibersys file, taking up space on your disk equal to
	the amount of RAM you have. Good if you don't have enough room on your C drive.)


Changing page file size (not recommended if you have less than 16GB of RAM)
WARNING Windows uses the page file for virtual memory. Do not change this unless you are sure what you are doing.
	* search for Adjust the appearance and performance of windows in the start menu
	* go to the advanced tab
	* Under virtual memory, click change
	* change to preferred size, or remove completely.
	* Optionally you can change the settings under Visual Effects.

Turn off useless windows features
	* Go to programs and features
	* Go to Turn windows features on or off
	* Uncheck Internet Explorer, Media Features, Games

Turn off System protection (stop windows from creating system images)
	* Control Panel\Recovery
	* Go to configure system restore
	* Disable system protection and click delete
	
Change computer name (this is what your name will be on your local network for example)
	* Right click This PC (in the left list in explorer) and click properties
	* click change settings under Computer name, domain and workgroup settings.
	* Under the tab computer name, click change on the bottom.
    
----------------------------------------------

for spotify users:
	if you have a small SSD its good to move the cache folder to another hard drive, so it does not take up space on your C drive.
	* In Spotify, go to Edit->Preferences, scroll all the way down and click show advanced settings
	* under "Offline Songs Storage" it says the current folder. FIND IT AND OPEN IT IN EXPLORER.
		- if its under "users/[yourusername]/AppData/Local the AppData folder will not be visible.
		  to access it press Win+R and type %appdata% and hit enter, and navigate from there.
		  Or just write the folder path into explorer.
	* Click Change Location and select a folder on another hard drive.
	* Lastly delete the old folder you opened in explorer.
    
    