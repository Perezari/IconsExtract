# IconsExtract v1.47

Copyright (c) 2003 - 2010 Nir Sofer

Web Site: http://www.nirsoft.net/utils/iconsext.html

Chinese Simplified/Traditional Translating languages Package: yanbog

Web site: https://www.engko.org

## Description
===========

The IconsExtract utility scans the files and folders on your computer,
and extract the icons and cursors stored in EXE, DLL, OCX, CPL, and in
other file types. You can save the extracted icons to ICO files (or CUR
files for cursors), or copy the image of a single icon into the clipboard.

![20200522091826.png](20200522091826.png)

## System Requirements
===================

Windows operating system: Windows 10, Windows 7/8, Windows 95/98/ME, Windows NT, Windows 2000, Windows XP, Windows 2003/2008/2012/2016/2019 Server, or Windows Vista.
IconsExtract can only extract icons from 32-bit executable files. It
cannot extract icons from 16-bit files.



## Versions History
================

1.47 26/09/2010

* Added -scanpath command-line option, which allows you to start
  IconsExtract with another base folder or wildcard. (For exmaple:
  iconsext.exe -scanpath "c:\windows")



1.46 13/04/2009

* The size of PNG based icons is now displayed properly. (In prevoius
  versions, the size was displayed as 0x0).



1.45 03/05/2008

* Fixed bug in scan mode selection.


07/03/2008 1.44


* Fixed the tab order in all dialog-boxes.
* Fixed the Esc key and 'x' close buttons of search and properties
  dialog-boxes.



1.43 22/02/2008

* Fixed the filename length limitation in the 'Search For Icons'
  dialog-box.
* Added support for typing filenames with environment strings (For
  example: %SystemRoot%\System32\shell32.dll)



1.42 21/12/2007

* The configuration is now saved into a cfg file, instead of the
  Registry



1.41 08/04/2006

* Fixed bug with large icons (256X256 or graeter) on properties window.



1.40 12/06/2005

* New option: Loaded all icons in the selected process.
* New option: File Properties.
* New column: Total size of the icon.



1.32 21/05/2005

* Added support for Windows XP visual styles.



1.31 01/12/2004

* Added support for translating to other languages.
* All dialog-boxes are now centered.



1.30 04/09/2003
Added command-line support.


1.21 06/06/2003
Automatically saves your last settings (windows size, your last search
options, and more) and loads them in the next time that you use this
utility.


1.20 30/04/2003
Added search filter (Icon size and number of colors).


1.10 16/04/2003

* Added support for cursors.
* Fixed bug: Error message when closing the main window during icons
  search.
* Fixed bug: Icons without numeric ID were not shown.
* The images of the icons are shown in properties window



1.00 02/04/2003
First release.



## License
=======

This utility is released as freeware. You can freely use and distribute
it. If you distribute this utility, you must include all files in the
distribution package including the readme.txt, without any modification !



## Disclaimer
==========

The software is provided "AS IS" without any warranty, either expressed
or implied, including, but not limited to, the implied warranties of
merchantability and fitness for a particular purpose. The author will not
be liable for any special, incidental, consequential or indirect damages
due to loss of data or any other reason.



## Using the IconsExtract utility
==============================

This utility is a standalone executable, and it doesn't require any
installation process or additional DLLs. Just run the executable
(iconsext.exe) and start using it.

Immediately after you run this utility, the "Search For Icons" dialog box
will be appeared. In this window, you should select the files or folders
that you want to scan, and the resource types you want to find (icons,
cursors, or both). You can also filter unneeded icons and get only icons
that contains images with specific size and number of colors.

You have 2 main search options:

1. Select only single file. For example: C:\WINNT\System32\shell32.dll
   You can manually type the filename in the text-box, or select it from
   a dialog box by clicking the "Browse Files" button.
2. Select multiple filenames by using wildcard characters (? and *).
   You can select the folder that you want to scan by clicking the
   "Browse Folders" button. If you check the "Search Subfolders"
   check-box, all the subfolders of the main folder will be scanned also.
   For example: if you type "c:\*.*" in the filename text-box, and check
   the "Search Subfolders" option, the IconsExtract utility will search
   for icons in all folders and files of your "C:" drive.

Notice: Searching for icons in an entire drive might take a few minutes,
and consume a fair amount of system resources. However, you can always
stop the search by pressing the "Esc" key or by clicking the "Stop" menu
item in the top-left corner of the window.

In order to start the icons searching, press the "Search For Icons"
button. IconsExtract will search for icons according to your selection in
the "Search For Icons" window. After the search is finished, the
extracted icons will be appeared in the main window of IconsExtract
utility.



## Saving icons into ICO files
===========================

In order to save the extracted icons into ICO files:

1. Select the icons that you want to save. You can press Ctrl+A in
   order to select all extracted icons.
2. Choose the "Save Selected Icons" in the 'File' menu, or press
   Ctrl+S.
3. In the "Save Selected Icons" window, type the folder for saving the
   icons files (You can also select it by using the Browse button)
4. Press the "Save Icons" button. All the selected icons will be saved
   into the folder you have selected.



## Copy a signle icon to the clipboard
===================================

You can also copy a single image of icon, and paste it to another
application. There are 2 options to do it:

1. Copy icon in standard dimensions (16 X 16 or 32 X 32): Select a
   single icon in the main window, and press Ctrl+C.
2. Copy an image of icons in other sizes: double click on a single
   icon, and the properties window, select specific image, and press the
   "Copy Selected Image" button.



## Searching more icons
====================

You can always make another search by using the "Search For Icons" option
in the File menu. You can also extract the icons of specific file simply
by dragging it from explorer window into the main window of IconsExtract
utility.



## Command-Line Support
====================

Starting from version 1.30, you can extract icons from files by running
IconsExtract with /save option.
iconsext.exe /save "source file" "save folder" [-icons] [-cursors]
[-asico]


source file
The file containing the icons you want to extract

save folder
The destination folder the save the extracted icons/cursors

-icons
Specify this option if you want to extract the icons from the file.

-cursors
Specify this option if you want to extract the cursors from the file.

-asico
Specify this option if you want to save cursors as .ico files.

Example:
iconsext.exe /save "c:\winnt\system32\shell32.dll" "c:\icons" -icons
-cursors

You can also use -scanpath parameter to start IconsExtract user interface
with the specified path or wildcard, for example:
iconsext.exe -scanpath "c:\windows\system32\*.dll"



## Translating IconsExtract to other languages
===========================================

In order to translate IconsExtract to other language, follow the
instructions below:
1. Run IconsExtract with /savelangfile parameter:
   iconsext.exe /savelangfile
   ```
   C:\Program Files (x86)\NirSoft\IconsExtract\iconsext.exe /savelangfile
   ```
   A file named iconsext_lng.ini will be created in the folder of
   IconsExtract utility.
2. Open the created language file in Notepad or in any other text
   editor.
3. Translate all string entries to the desired language. Optionally,
   you can also add your name and/or a link to your Web site.
   (TranslatorName and TranslatorURL values) If you add this information,
   it'll be used in the 'About' window.
4. After you finish the translation, Run IconsExtract, and all
   translated strings will be loaded from the language file.
   If you want to run IconsExtract without the translation, simply rename
   the language file, or move it to another folder.



## Feedback
========

If you have any problem, suggestion, comment, or you found a bug in my
utility, you can send a message to nirsofer@yahoo.com


## Translating languages Package
================================

IconsExtract is also available in other languages. In order to change the language of IconsExtract, download the appropriate language zip file, extract the 'iconsext_lng.ini', and put it in the same folder that you Installed IconsExtract utility.


Language|Translated By|Date|Version|
-|-|-|-|
Chinese Simplified|yanbog engko.org|21/05/2020|1.47
Chinese Traditional|yanbog engko.org|21/05/2020|1.47
Arabic|Shanaab|	26/01/2015	 
Brazilian Portuguese|	Siegfried Janke|	26/09/2010|	 
Bulgarian|	Starichok|	29/01/2015|	 
Croatian|	RandomGuyfromCroatia|	21/12/2015|	 
Czech|	Damned|	03/12/2013	 
Danish|	Aske Uhd Pennerup|	04/06/2005|	 
Dutch|	Jan Verheijen|	28/09/2010|	1.47|
Dutch|	Sander Lambregts|	27/09/2008	|1.45
Finnish|	Olli|	22/10/2007|	 
French|	Jean-Michel Gillion|	04/05/2008	 
French|	aMadEUs|	29/09/2010|	1.47
Galician|	Yako-_-|	21/07/2010	 
German|	??Latino?? auf WinTotal.de|	11/03/2014	|1.47
Ge Old Style|	J??rg-Peter Wessels|	25/04/2005	 
Greek|	George Georgiou|	05/05/2009	 
Hebrew|	Aron Don	|15/12/2011|	1.47
Hungarian|	Huzella Bal??zs|	19/07/2005	 
Italian|	Fabio Milocco|	06/07/2011	 
Italian|	Devil	|23/02/2014	|1.47
Japanese|	X-WORKS|	12/07/2005|	 
Norwegian|	Helge R??dne Skjeveland|	03/12/2005	 
Polish|	Szymon Ogrodnik	|14/06/2005	 
Portuguese|	Rui Morais|	10/09/2005	 
Portuguese| Brazil	Mark Nascimento - Bambu??|	15/05/2005	 
Romanian|	Jaff (Oprea Nicolae)|	15/02/2013	|1.47
Russian|	Starichok	|18/04/2006	 
Chinese Simplified|	renda|	26/02/2008	 
Slovak|	Michal "KuboF" Mat????ov|	04/05/2008	 
Spanish|	Carlos G??mez N????ez|	02/08/2006	 
Swedish|	Olle Jansson|	14/02/2012	|1.47
Chinese Taiwanese|	Republic Of China Taiwan|	17/12/2005	 
Chinese Traditional |	Sophina Liu|	29/08/2010	 
Chinese Traditional |	Mido|	05/08/2008	 
Thai|	??????????????????????????? ???????????????????????????|	25/03/2008	 
Turkish|	Selchuk Dursun|	22/08/2016	 
Valencian|	vjatv|	29/06/2005	 