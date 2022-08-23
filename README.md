# CMPINF0010 Skills Lab 
# Lab 1 - Introduction to Jupyter & the Stack

Welcome to the Lab session for CMPINF0010 Big Ideas in Computing and Information.

This week is going to focus on getting you oriented with the technology stack we will be using in the lab sessions for this course. The primary technologies we will be using is a platform called [Jupyter](http://jupyter.org) and the [Python](http://python.org) programming language. Jupyter is an open-source project that maintains a collection of tools for interactive computing. Python is an extremely popular general purpose programming language that has become widely used in the data science community. With their powers combined, Jupyter and Python make easy to interactively execute code to explore data. In the Big Ideas skills lab we will be doing just that!

More specifically, here are the main technologies you will be using in the skills lab:
* **Python** - A general purpose programming language that is both easy to learn and very powerful. 
* **JupyterLab** - JupyterLab is a web-based interactive development environment for Jupyter notebooks, code, and data.
* **Jupyter Notebooks** - The Jupyter Notebook is an open-source standard that allows you to create and share documents that contain live code, equations, visualizations and narrative text.
* **JupyterHub** - A multi-user version of Jupyter running on a remote server.


We will be using *JupyterLab* to create, edit, and execute *python* in *Jupyter Notebooks* in the lab sessions. We will be running JupyterLab on the [School of Computing and Information's](http://sci.pitt.edu) instance of JupyterHub. What this means is that you do not need to install any software on your own computer, everything will be running up "in the cloud" and you will only need a web browser to access it.


## Overview

This week's lab session has 5 parts.

1. Getting JupyterHub
   * Logging into the SCI JupyterHub (Prefered -> Do this)
   * Installing JupyterLab (Not prefered -> can be buggy/tepramental)
   * Binder (Break glass in case of emergency)
2. Using JupyterLab
3. Downloading Lab Materials
4. Introduction to Jupyter Notebooks
5. Uploading completed labs to Canvas

---

## Help Outside the "Classroom"

There is a new discord server for this class! Check out the course page to join!


---

## Part 1 - Getting JupyterHub

This is the first big task of the lab sections. Don’t worry, it’s not very difficult! There are 3 options to using JupyterHub for this class: connect to The SCI JupyterHub, installing it on your local machine, or using Binder. The easiest method is JupyterHub.

### What is the SCI JupyterHub?

The SCI Jupyterhub is actually a supercomputer! We’re accessing it for a couple reasons. It has a system installed on it that simplified working on the labs; it removes the need to install all the individual programs to open and edit Jupyter notebooks. This means regardless whether you’re accessing the hub from a PC or a Mac or a Tablet, you are able to write and execute anything you need in your notebook. Also, it’s really convenient to have everything chilling on the cloud; you’ll be able to access it from any machine as long as you have a browser and an internet connection.

The other nice thing about using JupyterHub is that it operates on its own file system.  This means everybody has a standard system to navigate, simplifying the process of debugging and fixing errors.

The downside is that you need to be connected to the Pitt VPN to acces the labs from off campus. Thankfully, since many of you are freshman, this shouldn't be too much of an issue!

#### How to login to the SCI JupterHub:

1.  If you are not on Pitt wifi, connect to the VPN. If you need help, instructions are [here](https://www.technology.pitt.edu/help-desk/how-to-documents/pittnet-vpn-pulse-secure-connect-pulse-secure-client)
    * Alternatively, you can connect virtually to one of Pitt's machines using these [instructions](https://www.technology.pitt.edu/services/virtual-lab)
2.  Go to https://jupyterhub.sci.pitt.edu.
3.	Log in with your Pitt credentials
    * Note: don't inlcude @pitt.edu, and your username needs to be **all lowercase** (e.g. abc12 is good, but ABC12 and abc12@pitt.edu are **not**)
4.	Verify yourself with Two Factor Authentication
5.	Click `Start my Server`
6.	Select `Host Process` from the dropdown (should be default), then hit `Spawn`
7.	That’s it, you’re in

Start my Server
![logging into jupyterhub](img/hub-login-1.png)

Spawn the Host Process
![logging into jupyterhub](img/hub-login-2.png)

Congratulations! You are now logged into JupyterHub. Your screen should (hopefully) look something like this:

![Jupyterlab screenshot](img/hub-login-3.png)

Welcome to Jupyter Lab!

### It didn't work!

There are two other options: download jupyterlab onto your machine, or access it via Binder.

### Downloading and installing Jupyter:

You can download the instructions from [here](setup/EnvironmentSetup.md) and follow them. All links are on the course webpage as well. Don't forget the [environment.yml](setup/environment.yml) file!

### Accessing labs via Binder

Don't worry, if you are unable to log into Jupyter Hub, we have set up an alternative on another JupyterHub called [Binder](http://mybinder.org). By clicking the link below you will be connected to a free instance of Jupyter running in the cloud. 

**Important Note:** If you are running on Binder and files or notebooks you create will be deleted after an hour of inactivity. Download anything you create to your local machine in order to preserve it (you will have to do this to hand in the lab exercises anyway)

* Click here if SCI Hub doesn't work:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pitt-sci-cmpinf0010/Intro-to-Jupyter/HEAD)

---

## Part 2 - Introduction to Using JupyterLab

Before we begin, please watch this video for a basic walk through for using JupyterLab so you can begin to acquaint yourself with its different features.
* https://www.youtube.com/watch?v=K2Yb1nXTmYM  (Ignore the stuff about MatrixDS)

### Creating a Notebook
Your lab sessions and exercises will mainly be using Jupyter Notebooks--which allow you to write pieces of code and/or markdown in an organized fashion. **We will be using Python 3.7, so be sure to select that when you are making a Notebook.** Remember to use good naming techniques when creating files and folders.

If you followed the instructions for downloading Jupyter on your own computer, then you should be familiar with opening a jupyter notebook through the Anaconda Navigator. Remember, make sure you tell Anaconda to open a Jupyter Lab session using the virtual environment that you imported from the course website.

### Understanding the File System
Just as your computer has a system of files with a hierarchical order to them, your files in JupyterLab is organized in a similar way. You can create folders to place lab materials and lectures in, then put folders inside of folders if you would like! You can navigate through these folders the same way you would on your local machine with windows explorer or finder.

If you're using the VPN/Virtual Lab or Binder, these files are not on your local machine, they live on the CRC JupyterHub (which has A LOT more space than your computer). You can upload and download files from this remote file system using the JupyterLab web interface.

### The Terminal and Text Editor
We will be using the terminal (or command prompt) for a variety of things during this class, but as explained an important use for it will be to download lab materials. Another good use for it is to navigate through files and run programs. 
The text file editor is useful for keeping information in, such as lists and certain data. We will learn more about doing this later in the semester!

---

## Part 3 - Downloading Lab Materials

Each week, the repository for the lab material will be on GitHub. Your TA will guide you in the process of accessing the materials (especially for this week), or if you have trouble, please come to office hours.

Assuming you are logged into JupyterHub, please do the following:

1. Click file &rarr; New &rarr; Terminal.
![new terminal](img/open-new-terminal.png)
It should open a window that looks something like this
![terminal window](img/new-terminal-window.png)
You should see a blinking rectangle - this is the cursor.
2. Copy and paste the the following command:
```shell
git clone https://github.com/pitt-sci-cmpinf0010/Intro-to-Jupyter.git
```
Your terminal window should look like this
![clone command](img/git-clone-command.png)
3. Hit enter and wait for the command to finish running. After it does, look to your left. You should see a new folder called `Intro-to-Jupyter`. Your file explorer on the right should look like this
![successful clone](img/lab-cloned-success.png)

Double click the new folder. You should now be able to see the following lab materials
- `README.md` - the README file document that you were reading for instructions on how to access the lab
- `Lab-Lesson.ipynb` - the Jupyter Notebook file with all of the exercises that you need to complete for this lab.
- Some other files that you can ignore

Your file explorer on the left should look like this

![lab materials](img/lab-materials.png)

---

## Part 4 - Introduction to Jupyter Notebooks

During the course of this, uh, course, you'll be completing your labs and final projects in the Jupyter notebook format. A **Jupyter notebook** is a combination of executable code, formatted text, and raw data.

A Jupyter notebook is, at its core, a bunch of *cells* on top of an interactive *kernel*. This explanation necessarily oversimplifies some things, but you can think of each notebook as having its own kernel that all of its cells can access and modify. So, for example, if you say `a = 123` in `Notebook1.ipynb`, any code cell within `Notebook1.ipynb` can see the value of `a`, but `Notebook2.ipynb` is unaware of the existence of the variable `a`. (For a counterexample, try clicking on the "Python 3" in the upper-right corner of a notebook once you're on JupyterHub. Have fun.)

The specific kernel we're using is an interactive version of Python 3 called IPython. This naming convention holds; the default Ruby kernel for Jupyter is called IRuby, for example. Many programming languages (including Java) have interactive kernels for creating notebooks, but we'll be sticking to Python 3 for this course. 

### Cells

Within the Jupyter notebook, there are three types of cells: code, Markdown, and raw. These cells can exist in any order within the notebook, and can be mixed and matched as you, the author, wish to do so. 

**Code cells** are the core of the Jupyter notebook's computation. They contain code that is run by the kernel. When you run a cell, any variables you assign are assigned for any code cell in the document, and any output your code produces is displayed directly below the cell.

![a sample code cell](img/scr1.png)

**Markdown cells** are the default way to display rich text, tables, images, GIFs, videos, and math markup. Markdown is a subset of HTML optimized for writing text quickly, and correspondingly is pretty lightweight. For example,

```markdown
# This Is A Header

Here's some **bold text**, and here's some *italics*. I can make a list like so:

* bullet
* points
* use
* asterisks

1. and
2. numbered
3. lists
4. just
5. use
6. numbers :)



I can also [link to things](https://www.pitt.edu) with parentheses and brackets. 

Adding an image is like a link, but more excited:
![image description goes here](https://media.giphy.com/media/3d3woRW2rHwyDvFKNg/giphy.gif)
```

It's easy to display `code` with backticks(\`). Longer code snippets get their own line:

    ```
    print("Here's a longer snippet of code.")
    a = 2
    b = 3
    c = a + b
    ```

You can see a full guide to Markdown [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), and we'll discuss it in more detail later in the course. But, for now, just know that you can write pretty text within a Jupyter notebook using Markdown cells.

**Raw cells** are the simplest cell type in Jupyter. They just contain raw, unformatted data that's not evaluated or changed in any way. If you want to include raw data points or text that's important to display as-is, raw cells are your best bet. We'll rarely use them in this course.

---

## Part 5 - Lesson & Exercises


The materials you downloaded in Part 3 contain a Notebook with instructions for this week's exercise. 

In the `Intro-to-Jupyter` folder, open the `Lab-Lesson.ipynb` Jupyter Notebook. Read through this notebook and follow the instructions. You will be instructed to create a new Jupyter Notebook with some Markdown text, images, and Python code. This is the notebook you will hand in using Canvas (instructions below).

---

## Part 6 - Uploading completed labs to Canvas

We will use [Canvas](canvas.pitt.edu) to let you upload your labs. 

1. First, if you used the SCI JupyterHub, Virtual Lab, or Binder, you're going to have to download the notebook to your computer.
    * On JupyterHub, right click on your exercise notebook on your file browser on the left
    * Click **Download** and save it somewhere

2. Then, go to Canvas to upload your lab.
    * In Canvas, click on our class
    * Go to Assignments
    * Click on the Skills Lab assignment for this week
    * Click **Submit Assignment** in the top right
    * Choose your Notebook file you saved/created/downloaded earlier (will end in `.ipynb`)
    * Hit Submit!

If you are confused, here is a [tutorial](https://community.canvaslms.com/t5/Student-Guide/How-do-I-upload-a-file-as-an-assignment-submission-in-Canvas/ta-p/274) on how to submit an assignment on Canvas.

**Note:** you can re-upload your lab as many times as you want before the deadline.

