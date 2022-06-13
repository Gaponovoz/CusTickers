# CusTickers
App for creating and sending custom and private stickers on Telegram

[##All the info and downloads - on my wesite! GitHub is for source code only.](http://gaponovoz.zapto.org/proj/custickers)


------------



This app is engineered in a horrifying way...
But here is **how to compile it from the very sources**:

  1.   **Compiling the main executable**. As mentioned in the list of libraries used to create the program, first you will need to download ARUEII by Longtion Software. You may use it for about 60 days for free, then clear the registry and install it again for 60 more days (if you need). After you installed it, open the project with extension ".aru". If you run the app in default ("debug") mode it will be automatically compiled and exe created. So, we have our main executable compiled successfully.
  2.  **Compiling modules-scripts**. We also need modules (secondary executables) to make this app run. Let us compile some batch-based ones first. These batches are a sort of modules of my app for performing both simple and perplexing operations. You may just use "Bat_to_exe_converter" from "Batch" folder but it is possible to download it from author's site. Reminder: list of all the libraries and software I used to create CusTickers is located below. So, we open every batch file in this app and compile it as "Windows 32-bit Invisible". Then put all the executables near the main file "autorun.exe". After that compile last script - TGfetcher. It is AHK script, to compile it, use ahk2exe converter.
  3. **Putting libraries**. CusTickers needs certain libraries to work correctly. They are SoX, ImageMagick and others (they all are listed in the List of open source and proprietary libraries and projects used). So, download the mentioned executables and libraries (use 32-bit portable versions). You can reference to the my (original) installation folder to find out the needed libraries and their names.
  4. **Making font installer for installer**. We should have 3 files near each other - "ubuntu.ttf" (font file), "FontReg.exe" (font verificator for Windows) and our executable we compiled from batch called "InstallFont". Also we need to have any version of WinRar installed. Select these 3 files, then click "Add to archive..." Check "Create SFX archive" and change archive type to "ZIP, no compression". Go to "Advanced", "SFX options". Here enter file "InstallFont" as a file to launch after unpacking and change the SFX mode to silent with no windows. Name the output SFX ececutable "FontInstaller.exe" and put into the source code folder.
  5. **Making an installer**. We use app "Install Creator Pro 2" for installer creation. Use that app as demo version. My project file is included in the source code archive. Just use it (name your source code folder "Source Code"!). Also put in the folder a Flash Player installer binary (any old 32 bit version) and call Flash.exe. Build the installer with compression preset "Maximum". Don't forget to delete unnecessary files from the source code folder like batch files. 
Here we go! The program is totally compiled with its installer.
 
 

------------


 
**List of Open Source and proprietary libraries and projects used to make CusTickers:**
1. file2clip by rostock
(for copying media to temporary clipboard with further sending from it)
3. SOX and (name in my project - "sticker-aud")
(for encoding Audio stickers)
4. ImageMagick (name in my project - stick-er)
(for editing custom user sticks to fit the interface of my app and to convert it for Telegram use)
6. Bat To Exe Converter by Faith Kodak
(for using windows batch commands as executable files)
8. FontReg by code.kilu.org
(for automatic installation of Ubuntu font when the program is being installed)
9. AutoHotKey compiled script
(for penetration-less putting stickers in the Telegram chat)
10. AR Pro Enterprise II (free demo version used)
(for creating GUI)
12. Adobe Flash (version ~2009, the original silent installer is included into my installer)
(for making that GUI run properly)
14. Install Creator Pro (free demo version used)
(for creating installation program)
15. 7zr 7z archiver command line version (name in my project - "custick")
(for sticker packaging feature)

------------




