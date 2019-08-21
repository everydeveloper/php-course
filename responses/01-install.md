# Initial Setup

PHP is a server-side language, so in order to make your code work you must put it on either a web-server or a local server. For the purposes of this tutorial we will install a local server called WAMP (for Windows users) or MAMP (for Mac users). You can also install LAMP server, if you use a Linux.

Noticing a pattern in these names? The only difference is the operating system. The -AMP part stands for Apache, MySQL, and PHP. We are using WAMP in this turotial, but use the version that matches your OS. 

Make sure you have a text editor installed before proceeding (such as [Atom](https://atom.io/), [Sublime Text](https://www.sublimetext.com/3), or [Notepad++](https://notepad-plus-plus.org/)).

## Install WAMP server (Windows)

- Go to [http://www.wampserver.com/en/](http://www.wampserver.com/en/) and click  "START USING WAMPSERVER"
- Choose either the 64bit or 32bit version.  (Most machines should run the 64 just fine but if in doubt choose 32)
- Once your server is installed open a browser and go to [http://localhost](http://localhost) if it works then your install is finished.
- Make sure to note where your php files are located in WAMP ie: C:\\wamp64\www (move or delete all files in this folder now)

## Install MAMP server (Mac)

- If you are a Mac user, go to [https://www.mamp.info/en/downloads/](https://www.mamp.info/en/downloads/) and select the MAMP version that works for your computer.

## Clone course repository

You will be storing the code for this project in [this repository]({{ repoUrl }}). Before we go any further, navigate to the www folder in your terminal (which should be empty now). Clone your template project into this folder, using [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git):`git clone {{ repoUrl }}.git`

Refresh your browser, and make sure you see folder for the php-course. If it worked, close this issue for the next step.