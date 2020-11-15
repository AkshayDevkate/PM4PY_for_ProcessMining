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
  
  
  
  
 
 
