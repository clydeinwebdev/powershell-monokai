# powershell-monokai
Customized (PS) PowerShell Monokai Color Scheme

##Requirements

* Windows 7 & 8
* Powershell 2
	```
 	> $PSVersionTable.PSVersion
	
	Major  Minor  Build  Revision
	-----  -----  -----  --------
	2      0      -1     -1

 	```


##Steps

1. Clone repo
	```
	> git clone git://github.com/ntwb/posh-monokai.git
	```
1. Download Open Type Fonts [Adobe Source Code Pro](https://github.com/adobe-fonts/source-code-pro)
1. Install Open Type Fonts
	1. Navigate to the folder that contains the fonts you want to install.
	1. Select the fonts you want to install. You can click to select one font, Control-click to select several fonts, or Shift-click to select a contiguous group of fonts.
	1. Right-click the selected fonts and choose "Install."
	1. The fonts are now installed and will appear in the font menus of your applications.
1. Merge ```HKCU-Console.reg```. This will register Monokai colours for Powershell
	1. Click the "Start" menu.
	1. Type "regedit" in the "Search" box and press "Enter." Select "Regedit" from the list to open the program.
	1. Click "File" on the menu bar and select "Import" from the drop-down menu.
	1. Select the registry file you wish to merge with the existing registry and click "Open."
	1. Note: ```Registry files may also be merged with the system registry by double-clicking the REG file.```
1. Merge ```register-console-font.reg```. This will register Open Type Fonts as a console font
1. Install posh-git. Clone, change directory, install then refresh the powershell profile
	```
	> git clone https://github.com/dahlbyk/posh-git.git
	> cd posh-git
	> .\install.ps1
	> $PROFILE
	```

##Other Links
* [orangwarp](https://github.com/orangewarp/posh-monokai)
* [dahlbyk](https://github.com/dahlbyk/posh-git)
* [ntwb](https://github.com/ntwb/dotfiles)