# Arduboy-Uploader-script
This is an Arduboy uploader script written in python. It was made for Macs, probably works on Linux and possibly could be modified to work on Windows

## Installation
1. Clone repo and put the python script in `~/bin` (create it if it does not exist)
2. Open the script using any text editor  
Note:  
You need to have the Arduino IDE for this to work
3. Go to the Arduino IDE and open preferences (`command-comma` on Macs)
4. Find `Show verbose output during:` and select the `upload` box (You can disable this later but i think it looks cool so don't)
5. Upload an empty sketch. (I recommend the hello world sketch which is part of the Arduboy2 examples)
6. Click upload and find `PORTS{...}` and copy the line below the last one of those lines
7. Go back to the text editor and find a looooong line of code
8. Paste the line which you copied from the IDE in to the `os.system`'s arguments
9. Find `-Uflash:w:`...`:i` then replace the ... with `{file_name}`
10. Find `-P` and then copy the path which comes after the `-P`
11. Replace the thing you just copied with `{ARDUBOY_LOCATION}`
12. Find a line called `ARDUBOY_LOCATION = `
13. Replace the text between the quotes with the path you copied just now
14. Save and quit
15. Check if it works using the Example tab

## Example
To upload a hex file, open terminal an type in `ArduboyUploader ` and type in the path to the file (e.g. `~/Downloads/ardutosh.hex`)  
Plug in your Arduboy and turn it on  
Press enter. If you see errors, check that required libraries are installed  
If you can't figure it out, feel free to contact me at ileshkt@gmail.com
