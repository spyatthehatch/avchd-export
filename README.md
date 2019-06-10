# avchd-export
## About
This is a bash script to export MTS files from AVCHD and losslessly convert them to mp4 files.  It requires FFMPEG to convert MTS files to mp4 files.  This will loop through all MTS files in an Sorry PC users, this solution is for Mac OSX only!

## The Easy Way
Watch the youtube video for instructions on how to install and use the avchd-export.bsh script:
https://www.youtube.com/channel/UC5V6s5bXc8nI7FU9PKIya8Q

## Installation
1. Download FFMPEG at https://evermeet.cx/ffmpeg/.<br>
2. Or, if that URL makes you nervous: https://ffmpeg.org/download.html#build-mac, click the Apple icon and choose "Static builds for macOS 64-bit."  You'll see that we're at the URL in Step 1, but whatever.
3. Download either the release or snapshot as a DMG. Which should you choose?  It's up to you.  The release will be more stable (potentially), but the snapshot will have bug fixes.  Between you and I, I chose the release version.  Just remember, "Download as DMG."
4. Create a new directory called, "FFMPEG" in your Applications directory.  Open the DMG file and drag the ffmpeg file into your new directory.  When done, it should be located at /Applications/FFMPEG/ffmpeg.
5. Download the avchd-export.bsh script to wherever your little heart desires.
6. If you decided not to listen to Step 3 and put the ffmpeg binary at some other location, update the FFMPEG variable in the avchd-export script (read the comments).

## Usage
The script is executed as:
<b>./avchd-export [import directory] [optional:export directory]</b>

1. Open the directory with your MTS files.  This can be sticking an SD card in the reader:<br>
  a. Go to PRIVATE.<br>
  b. Right click AVCHD, Show Package Contents.<br>
  c. Right click BDMV, Show Package Contents.<br>
  d. Enter STREAM, by double clicking.  TA-DA, MTS files!  And, if at this point you were wondering: Sony and Panasonic came up with the AVCHD format.
2. Open a termial.  Go to Applications, Utilities, Terminal.  Go to the directory where you downloaded the avchd-export.bsh script.
3. Execute the avchd-export.bsh script: Type:" ./avchd-export.bsh " (note the space!) and drag the window with your MTS files into your terminal.  It should add the directory path for you so it looks something like: "./avchd-export.bsh /Volumes/Untitled/PRIVATE/AVCHD/BDMV/STREAM"  Before you hit enter, read the optional Step 4.
4. Optionally: add the location where you would like the exported files to go.  By default, the script will put them in a new directory called avchd-export.
5. Pull the trigger (this means, press Enter).  Wait.  Profit.
  
