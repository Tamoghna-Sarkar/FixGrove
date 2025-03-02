# After following the steps (reflashing and running the script) I still get the error below on step 4: 

##  import di_i2c
ModuleNotFoundError: No module named 'di_i2c'

Furthermore, as I ran step 3, I got the message below several times: 

error: externally-managed-environment

× This environment is externally managed
╰─> To install Python packages system-wide, try apt install
    python3-xyz, where xyz is the package you are trying to
    install.
    
    If you wish to install a non-Debian-packaged Python package,
    create a virtual environment using python3 -m venv path/to/venv.
    Then use path/to/venv/bin/python and path/to/venv/bin/pip. Make
    sure you have python3-full installed.
    
    For more information visit http://rptl.io/venv

It seems I cannot install python packages unless I use venv. 

Any suggestions? 

# answer:

might be a python3 issue, you can try running
python3 -V
to see if you have python3 installed, since some dependencies are python3. Install it using "apt" if not.

if that doesn't help try run running the command in my comment above, I updated it with some fixes and combined the script to do both step 3 and step 4. Make sure you're on stable internet connection as sometimes it will fail to pull something from the Internet if connection is intermittent. 

if it still doesn't work, you can do the reimagining as in lab1 and then run the script I provided without running any other command prior. 

hope it helps, let me know if there's any issues with the setup script. 
