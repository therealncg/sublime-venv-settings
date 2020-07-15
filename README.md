# sublime-venv-settings
Venv settings for the Sublime Text 3. For Linux (Ubuntu) and Windows 10

# Ubuntu

### Terminal Code

    python3 -m venv /home/rafi/Desktop/test
    
  > You may need to type this down code, if the terminal ask you to type this, go ahead and do what it says!
  
    sudo apt-get install python3-venv
   > If it is not asked no need to type the above line
    
* To activate Venv [source /location/bin/activate]

      source /home/rafi/Desktop/test/bin/activate
    
> Alternate way to activate Venv [dot(.) /location/bin/activate]

      . /home/rafi/Desktop/test/bin/activate

#### Venv path in Linux (Ubuntu 20.04 LTS):
   Tools > Build System > New Build System...

    {
    "cmd": ["/home/rafi/Desktop/test/bin/python3", "-u", "$file"],
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
    "quiet": true
    }


# Windows 

### Command Prompt(cmd) Code

    python -m venv C:\Users\Rafi\Desktop\test
    
* To activate Venv [copy file path of activate.bat]

      "C:\Users\Rafi\Desktop\test\Scripts\activate.bat"

#### Venv path in Sublime Text 3 Windows 10:
   Tools > Build System > New Build System...
      
      {
      "cmd": ["C:/Users/Rafi/Desktop/test/Scripts/python", "$file"]
      }
   *Remember the forward slashes*

