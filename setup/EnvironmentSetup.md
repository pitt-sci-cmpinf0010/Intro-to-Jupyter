# Installing Jupyter Lab

## Install git
* Git for [Windows](https://git-scm.com/downloads) (Use default settings)
* Git for macOS (two options):
  * Install [Xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12) (Xcode comes with Git)
    * App takes up 11 GB of storage. If you are low on memory, try installing Homebrew.
  * Install [Homebrew](https://brew.sh)
    * Follow [macOS Git instructions](https://git-scm.com/download/mac) for Homebrew
    * Not necessary if you installed Xcode (but still potentially useful down the line!)

## Install Anaconda
* [macOS](https://www.anaconda.com/products/individual#macos)
  * Download the graphical macOS installer. (Keep default settings)
  * Follow the instructions presented by the graphical installer
* [Windows](https://www.anaconda.com/products/individual#windows)
  * Download the graphical installer. (Keep default settings)
    * Once installed it will take a bit to open up for the first time.

**Note:** Both the Mac and Windows installers will ask you if you want to install PyCharm. This is an application that some people use to make coding more convenient. You don’t have to download it, and we certainly won’t be using it in this course. But it won’t hurt to download it, and it could be useful for future python programming courses. Either way, don’t sweat it.

## Find and Open JupyterLab
* Once you have Anaconda installed, open up the Anaconda Navigator by searching in your computer search bar for the Anaconda Navigator application. 
* After opening up the Anaconda Navigator, you will immediately see several applications. Click the blue Launch button under JupyterLab application. We will be using JupyterLab throughout the semester.
* Once JupyterLab opens successfully in a new window, shut it down by completing the following steps:
  1. First, make sure you have saved your work. Do this by going to the top left and clicking File → Save
  2. If you haven’t saved the notebook before, you may want to use File → Save as
     * You can also save by clicking the floppy disk icon (and yes, I realize that many of you have probably never seen a floppy disk in your life 😂)
  3. In the top left of the JupyterLab window, click Kernel → Shut Down All Kernels
  4. In the top left of the JupyterLab window, click File → Shut Down

**NOTE:** You will want to perform these steps every time before you close the JupyterLab or JupyterNotebook tab.

## Using the cmpinf0010 Environment
1. Find the environment.yml file in this directory
  * The environment name default will be called cmpinf0010. Don’t change this please
2. In the Anaconda Navigator window, click the Environments tab on the left side toolbar.
3. Click the import button on the button left of the Environments window in the Anaconda-Navigator.
4. Use the file logo in the pop-up window to find/navigate to the environment.yml file
5. Click import.

**NOTE:** On the bottom right hand side of the Environments screen you will see a loading bar - wait until the cmpinf0010 environment is completely imported. This may take awhile, and that’s ok! You may want to make sure your computer is plugged into a charger.

## Open JupyterLab via the cmpinf0010 environment:
1. Once your cmpinf0010 environment is fully imported, switch back to the Home tab in the Anaconda Navigator.
2. In the top, make sure the correct environment is selected in the dropdown box next to “Applications on”. Select cmpinf0010 if a different environment name is there.
3. Launch JupyterLab
4. If your JupyterLab opens in a new window, click Python 3 under Notebook.
5. Type the following into the empty cell in the JupyterNotebook: `import geopandas`
   1. Hit the Shift and Command/Control (Shift+Command/Control) keys at the same time while still clicked in that cell.
   2. If you do not receive any errors, you have successfully imported the environment for this course. 

## Verify packages on the cmpinf0010 environment
1. Open the environment tab in Anaconda-Navigator. Make sure the cmpinf0010 environment is selected. On the right side, you will see all the packages installed on the cmpinf0010 environment. 
2. In the search bar search for scipy Verify that is installed. Then search for geopandas, pandas, matplotlib. Verify there are all installed.
3. If there is any package you find missing, please alert a TA.
	

