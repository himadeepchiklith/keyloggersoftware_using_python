# keyloggersoftware_using_python
Advanced Keylogger in Python with screenshot, microphone, webcam pictures taking capabilities and also Collects Network/Wifi Info, System Info, Clipbaord Data, Browser History and then send these files through email.

Installation & Running of this Keylogger:

1. Download Python and Install it.
2. Make sure all the associated modules are installed. I've added all the modules in the requirements.txt file.
3. If any of the module is not in the requirements.txt file then open Command Prompt & type

pip install ModuleName

4. At line 91 in the main file enter your full email instead of narashikamaru1516@gmail.com.
5. At line 92 in the main file enter the password for that email account.
6. Make sure in the gmail account settings that the allow less secure apps is on.
7. Open up a Command Prompt and Change to the directory the program is placed and execute the advancedkeylogger.py file.
8. Open the graphical file manager and go to the C://Users/Public/Logs directory to watch the program in action.
9. After files are encrypted and sent to email, download them and place them in the directory specified in Decryptor.py and run the decrypt file in command prompt.

#Working:
1. Creates a directory to temporarily store information to exfitrate
2. Gets all the essential network information -> stores to log file (takes about a minute)
3. Gets the wireless network ssid's and passwords in XML data file
4. Retrieves system hardware and running process/service info
5. If the clipboard is activated and contains anything -> stores to log file
6. Browsing history is retrieved as a JSON data file then dumped into a log file
7. Then using multiprocessing 4 features work together simultaniously: (Timeouts and ranges can be adjusted)
8. Logs pressed keys
9. Takes screenshots every 15 seconds
10. Records microphone in 10 seconds segments
11. Takes webcam picture every 5 seconds
12. After all the .txt and .xml files are grouped together and encrypted to protect sensitive data
13. Then by individual directory, the files are grouped and sent through email by file type with regex magic
14. Finally the Log directory is deleted and the program loops back to the beginning to repeat the same process.
