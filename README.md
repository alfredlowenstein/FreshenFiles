# FreshenFiles
Windows Backup of Directories and Files 

FreshenFiles will back directories and files.  You can skip specific file names, 
files which match a pattern (using wildcards), and files which start with 
specific characters.  It is fast because will only copy updated files.


-----NOTES-----

1.  The first time you run **Freshen Files**, any and all files/directories may 
not exist in the backup directory, and you should expect a lot of time to complete.  
However, subsequent backups will only have to freshen (i.e., update) 
files/directorieswhich have changed, so the update will be very fast.  
I backup 60,000 files in less than a half a minute.  However, the 
first backup took an hour or so. 

2.  During installation, a sample file with a list of directories and 
file was written to the desktop.  That SampleFile, SampleListOfDirectoriesToBackup.txt, 
contains directions about editing the file.  You need to edit this 
file to list all directories/files that you want to backup.  

2a. You can rename, copy, or move the SampleFile to whereever you wish.  
You can create many different SampleFiles that backup different stuff. 

2b.  AFTER INSTALL, THE DEFAULT PATH IN THE UPPER RIGHT TEXTBOX, 
**Select File with List...**, must be changed to point at a SampleFile created 
in the above step.

3.  To enter/change a directory/file in this window, you can either: 

   o  type or copy text into the field
   o  press the button next to the field
   o  drag/drop it in the field

4.  If you change the settings in this window and to want to save them, click **Update Settings**.

5.  If you are not sure that you trust your settings, you can test them by with the 
**List Only, No Copy** checkbox.  When you click a Freshen button, the files/directories 
that would be copied will scroll in this window.  When the checkbox is cleared, 
then a Freshen button will do the updating.


==============Here is a sample backup file to show what can be done============



'This is a sample backup file.

'Blank lines are ignored.
'Lines that start with a backtick (i.e., the first character in this line) are ignored.

'Lines with the following comma separated <keyword>,<value> pairs do the following:

'Keyword                            Value
'------------------------------     -------------------------------------------------
'DIRECTORY_TO_FRESHEN               Backup the directory
'FILE_TO_FRESHEN                    Backup the file on that line.
'FILE_EXTENSIONS_TO_EXCLUDE         Exclude backup of files with this extension
'                                   Note that you need to include a period (.).
'FILES_TO_EXCLUDE                   Exclude backup of files with this filename.
'FILES_TO_EXCLUDE_THAT_START_WITH   Exclude backup of files that start with this filename

DIRECTORY_TO_FRESHEN,c:\dad
DIRECTORY_TO_FRESHEN,c:\mom
DIRECTORY_TO_FRESHEN,C:\Utility
DIRECTORY_TO_FRESHEN,C:\MyPictures
DIRECTORY_TO_FRESHEN,C:\Download
DIRECTORY_TO_FRESHEN,C:\MusicNew
DIRECTORY_TO_FRESHEN,C:\MusicWave

FILE_TO_FRESHEN,C:\Windows\msdfmap.ini
FILE_TO_FRESHEN,C:\Joe\help.txt 

'Files to exclude
FILE_EXTENSIONS_TO_EXCLUDE,.BAK
FILE_EXTENSIONS_TO_EXCLUDE,.LNK

FILES_TO_EXCLUDE,FOLDER.JPG
FILES_TO_EXCLUDE,DESKTOP.INI

FILES_TO_EXCLUDE_THAT_START_WITH,~
FILES_TO_EXCLUDE_THAT_START_WITH,ALBUMART

'The following lines are commented out.  They are ignored.
'DIRECTORY_TO_FRESHEN,C:\Music34
'DIRECTORY_TO_FRESHEN,C:\Video
