# PM4PY_for_ProcessMining

 ## PM4PY for Process minig Installation guide 
 
  __Windows Operating System__
  
  This section is divided into four parts that are required to get PM4Py running.
  
   1. Install Windows C / C++ compiler 
      A fundamental package to install in order to make dependencies work is the Microsoft Visual C++ Redistributable, that can be found at the following URL
  [Click Here to Download!](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)
  
  Only in Python 3.6, since we are using some dependencies, e.g. ciso8601, you also need a C/C++ compiler. We suggest to install the Microsoft Visual Studio 2017 compiler that is available for free through the following URL
  [Click here to Download!](https://visualstudio.microsoft.com/de/thank-you-downloading-visual-studio/?sku=Community&rel=15)
  
   2. Install GraphViz
    
   For the purpose of visualization with pm4py, GraphViz installation is required. To install GraphViz, the installer on this page could be used
   [Click here to Download GraphViz!](https://graphviz.org/download/)
   
   After installation, GraphViz is located in the program files directory. The bin subfolder of the GraphViz directory needs to be added manually to the system path. For Windows 10, we suggest the following article in order to have an explanation of how to add a new folder to the system path [Adding a folder to system path](https://stackoverflow.com/questions/44272416/how-to-add-a-folder-to-path-environment-variable-in-windows-10-with-screensho)
   
   3. Install Anaconda or Miniconda 
   
   Anaconda is a free and open source distribution of the Python programming language for data science and machine learning related applications. If you have not install any variant, we suggest Miniconda. [Click here]() to install Miniconda.
   
   During the installation of the Miniconda distribution, it is important to select the addition of Miniconda Python to the system path option. This allows us to get easy access to Python from the command line / Powershell.
   
   > C:\>cd C:\Users\johndoe\pm4py-source
  
  4. Install PM4PY

   In order to install PM4Py and its dependencies, the following command should be executed:
   
   >pip install pm4py
   
  5..zip file
  
  A .zip file containing Windows 64-bit Miniconda 3.8 distribution and all the dependencies already installed could be found at clicking
  [Click here to download .zip file](https://drive.google.com/file/d/1KzIntSeIPJrjSzsrD93MZHAW4au-Wbgm/view)
  
 
 
 __Install PM4PY on macOS__
  
  You can chosse between an Docker image or the classical installation process.
  
  1. Installation via Docker
  
  A Docker image is available on the Docker hub and could be retrieved through the command.
  
  >docker pull javert899/pm4py:latest
  
  It could be then run trough the following command.
  
  >docker run -it javert899/pm4py:latest bash
  
  2. Classical Installation
  
  This section provides you help to run PM4Py without using Docker.
  
   a. Install Anaconda/Miniconda
  
   Anaconda 2020.07 (if not already installed; it is not necessary if Miniconda is installed) could be retrieved by [clicking here]().

   Miniconda (if not already installed; it is not necessary if Anaconda is installed) could be retrieved by [clicking here]().
   
   b. Install the PM4Py package
   
   In order to install PM4Py and its dependencies, the following command could be provided:
   
   >pip install pm4py
   
   To check if everything is done correctly, the following command can be used.
   
   >python -c "import pm4py"
   
   
   
   __Installing PM4PY on Linux Operating System__
   
   You can choose between an Docker image or the classical installation process.
   
   1. Installation via Docker
   
   A Docker image is available on the Docker hub and could be retrieved through the command.
   
   >docker pull javert899/pm4py:latest
   
   It could be then run trough the following command.
   
   >docker run -it javert899/pm4py:latest bash

   2. Classical Installation
   
   a. Install C/C++ compiler
   
   Most distributions default install include already the gcc and g++ compilers, respectively compiling C and C++ code. In order to check the presence of gcc and      g++ on your current distribution, along with their version, one of following commands can be used.
   
   >gcc -v
   
   >g++ -v
   
   If they are not installed, refer to your distribution support for instructions on how to install them.
   
   b. Install GraphViz
   
   The presence of GraphViz is required on the system. To check the presence of GraphViz, please give the following command.
   
   >dot -h
   
   If GraphViz is not installed, you will get an error from the output of that program. If GraphViz is not installed, you will get an error from the output of that    program. To install GraphViz, a command depending on the distribution should be given. We provide some commands for the most widely used distributions.

   For Debian/Ubuntu, the following command can be used:
   
   >apt-get install graphviz
   
   c. Install Tkinter
   
   Tkinter is required by Python but could not be installed with pip. It is required to install it through the distribution package manager.

   For Debian/Ubuntu, you can use the following command:
   
   >apt-get install python3-tk
   
   d. Other libraries
   
   Some other libraries are required to be manually installed on some platforms (like ARM)
   
   >apt install libblas-dev
   >apt install liblapack-dev
   >apt install libsuitesparse-dev
   
  e. Install Anaconda/Miniconda
  
  Miniconda (if not already installed; it is not necessary if Anaconda is installed) could be retrieved by [clicking here]().

  The 64 bit installer could be executed from the command line using the following instruction;
  
  >root@debian:~# bash Miniconda3-latest-Linux-x86_64.sh
  
  As the first step in the installation of Miniconda, it is required to read the license agreements. Press Enter key in order to read them, move with up and down     arrow keys in order to read the points, and then click q in order to quit the license agreements and accept/deny (yes/no) that.

  Then, a path for the installation of Miniconda is required. The proposed path, that is inside the user directory, is proposed and could be accepted as-is. Then,   Miniconda asks if the user wants to add executables to the user path, it is convenient to say yes here
  
  f. Install the PM4Py package
  
  In order to install PM4Py and its dependencies, the following command could be provided:
  
  >pip install pm4py
 
