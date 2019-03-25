# Virtual environment


For creating different packages we require variety of modules(supporting packages) to be installed therefore we need virtual env to keep the things seperate and precise, there comes the pythonic way of having a virtualenv. Kindly subscribe star the respo and request for more in the community.

  - Windows
  - Mac/ Linux
## Checking which python package is installed : 
-       pip --version

If pip is installed proceed...  
# Installation!

  If you have python already installed in your local machine / server, just install the virtual environment package using the following  
  
  - Windows:
    -     pip install virtualenv 
  - Mac/ Linux
    -     sudo pip install virtualenv
    -  if you get an error in the above command use the following for mac/linux:
    -     sudo -H pip install virtualenv 

## Using Virtualenv
If you recently installed virtualenv, you need to restart or reinstantiate the commandline / terminal to have the new packages be linked.

-   Create your project directory by explorer or use the following commandline argument
    -       mkdir [YOURPROJECTNAMEHERE]
- After creating that specific directory, browse inside it using explorer or the following command line argument
    -       cd [YOURPROJECTNAMEHERE]
- For Creating a virtual environment in that specific Project, use the following in terminal/commandline:
    -       virtualenv  [ENVIRONMENTNAMEHERE]
- OR
  
    -       venv [ENVIRONMENTNAMEHERE]
Keep in mind that the []* names can be replaced by anyname you like (recommended : env as a name convention)

### Virtualenv Structure
The following is the diretory of virtual environment

    ---> Include # Consist of C/C++ based build Packages 
    ---> tcl
    ---> Lib
    ---> Scripts
        |
        ---> activate.bat
        ---> deactivate.bat

Two files in the directory Scripts are important which are activate and deactivate batch based files, these files will be used for the activation and deactivation of a virtual environment.

### Activating Virtualenv

  - For activating the virtualenv, browse in the the [ENVIRONMENTNAME] using commandline / terminal
    -     cd [ENVIRONMENTNAMEHERE]
  - In Windows Browse to 
  
            -             [ENVIRONMENTNAMEHERE] / Scripts /  and type "activate"
  -  In linux/ MacOS based version if there is a bin folder, always go for

            -   [ENVIRONMENTNAMEHERE] / Scripts / activate .
            
            
The terminal will prompt a base "(env)" in the left most cursor space which indicated that you are in a specific virtual env.

### Installing packages

You can also install packages the same way you do in python pip:

    - pip install [PACKAGENAME]

### Requirements File
For Generating a requirement file, you can simple use the freeze command dumping into a raw file. Keep in mind it is recommended to use after activating the specific Project Virtual env.

        - pip freeze >> requirements.txt

### Installing from Requirement File in Venv
There are N numebr of Scenarios where you want to install 100's of packages for a project or migerate from a different project or location so to install from requirements file, you should activate a virtualenv and then use 


        - pip install -r requirements.txt

### Deactivating Virtual env

For Deactivating Virtual env, just simply type "deactivate" in that specific Console/terminal where Virtual environment is activated.



For more information it is recommended to browse the virtualenv libraries presented by pip. 
Star : repository
github : shafaypro
youtube : imshafay
