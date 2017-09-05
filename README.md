1. Install windows
	* Make sure that only the disk you intend to have windows on is the ONLY disk on the system. 
		You can add disks after the installation. This is because windows tends to put system files on other
		disks if they are available.

2. Install drivers (windows 10 helps with this)

4. Download and Install Ninite. Ninite is an all in one installer for commonly used software.
	* go to ninite, check all the programs you want, click download and install.

----------------------------------------------
5. Windows settings:

Increase privacy:
	* https://www.youtube.com/watch?v=5x2VTN4jjIE (tek syndicate)
		(The uninstalling of windows features also uninstalls things like calculator, but there are better alternatives anyway)

Turn off skype ads:
	* search for "Internet Options"
	* go to security, click restricted sites and then sites, block g.msn.com and apps.skype.com

Turn off hotkey for sticky keys
	* press shift x5 and turn of sticky keys

Remove OneDrive (https://www.windowscentral.com/how-remove-onedrive-file-explorer-windows-10)
	* start CMD as administrator
		* FOR 64BIT WINDOWS: paste "%SystemRoot%\SysWOW64\OneDriveSetup.exe /uninstall" (WITHOUT THE QUOTES) and press enter
		* FOR 32BIT WINDOWS: paste "%SystemRoot%\System32\OneDriveSetup.exe /uninstall" (WITHOUT THE QUOTES)  and press enter
	* open regedit (win+r and type regedit and hit enter)
	* Navigate to the HKEY_CLASSES_ROOT\CLSID\{018D5C66-4533-4307-9B53-224DE2ED1FE6} key
	* open System.IsPinnedToNameSpaceTree and change it from 1 to 0.

Language for non unicode programs
	* Go to Control Panel\Region\Administrative
	* Change system locale to English (United States)
	* Go to tab Location and change Home location to your country

disable ctrl+shift hotkey that changes input language
	* Open Control Panel, go to "Clock, Language and Region" -> "Language" -> "Advanced Settings"
	* click "Change language bar hot keys".
	* Under the Advanced Key Settings tab, under "Hot keys for input languages", remove all hotkeys.
	
Folder options
	* Open File Explorer and in the upper left corner, select file -> Change folder and search options
	* Set standard startup folder to This PC
	* Disable folder history
	* disable hide extensions for known file types
	* Delete library folders

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


Changing page file size. The page file takes 
NOTE-Windows uses the page file for virtual memory. Do not change this unless you are sure what you are doing.
	* search for Adjust the appearance and performance of windows in the start menu
	* go to the advanced tab
	* Under virtual memory, click change
	* change to preferred size, or remove completely.
	* Optionally you can change the settings under Visual Effects.

Turn off useless windows features
	* Go to programs and features
	* Go to Turn windows features on or off
	* Uncheck Internet Explorer, Media Features, Games
	* Press Ok

Turn off System protection (stop windows from creating system images)
	* Control Panel\Recovery
	* Go to configure system restore
	* Disable system protection and click delete
	
Change computer name (this is what your name will be on your local network for example)
	* Right click This PC (in the left list in explorer) and click properties
	* click change settings under Computer name, domain and workgroup settings.
	* Under the tab computer name, click change on the bottom.

for spotify users:
	if you have a small SSD its good to 
	another hard drive, so it does not take up space on your C drive.
	* Go to Edit->Preferences, scroll all the way down and click show advanced settings
	* under "Offline Songs Storage" it says the current folder. FIND IT AND OPEN IT IN EXPLORER.
		- if its under "users/[yourusername]/AppData/Local the AppData folder will not be visible.
		  to access it press Win+R and type %appdata% and hit enter, and navigate from there.
		  Or just write the folder path into explorer.
	* Click Change Location and select a folder on another hard drive.
	* Lastly delete the old folder you opened in explorer.
	
----------------------------------------------
6. Install:
	Discord
	Greenshot
	ImageGlass
	Notepad++
	Paint.NET
	WinDirStat
	Visual Studio 2017 community
	Unreal Engine
	Blizzard games launcher
	Github
