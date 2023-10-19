# Preparation
> [!NOTE]
> _**The following guide is part of the Counter Hydro-Cartographies workshop under the Gray Area Festival 2023: Plural Prototypes and the C/Change Initiative.**_
> _**Click [here](../) to go to the workshop’s main GitHub page.**_

Before attending our hands-on workshop, all participants are invited to follow the contents of this guide as it covers the preparation of computational requirements and installation of necessary software tools and packages, as well as assumptions on behalf of assumed technological literacy from workshop-takers, to follow and complete its main goals and objectives.

## Assumptions
While participants are not expected to have advanced literacy on computer-handling, it is desired that participants have a familiarity in relation to the knowledge necessary to read, write, and understand basic Python 3.x programming in an Integrated Development Environment (IDE) of their liking, as well as the creation of a Google account from which a Google Cloud user will be linked to the participant’s local machine in order to call and use Google Earth Engine’s Python API, which is from where workshop productions will be extracted from for the intended exercises. Having this expectation covered, following this guide will set you ready to achieve this workshop’s objectives under the authors’ preferred and tested configurations and environments.

## Prerequisites
> [!IMPORTANT]
> We remind readers of these guides that they were written for a workshop taken in late 2023; by the time you read them, these might be outdated.

The hands-on workshop requires the following hardware, software, and services prerequisites fulfilled. While following this guide will get you these prerequisites in check, do note that you may already have them set; either way, at least a skim through it is recommended so as to get the participants familiar with the tools necessary to use in upcoming guides under this workshop.

### Hardware
#### Acces to a Personal Computer
Although with the advent of new innovative forms of technology such as current-day phones, tablets, and IoT devices have put forward into question how a computer looks like, what we mean with _Personal Computer_ is a machine that is capable of running a Windows (10 or 11), MacOS (from Catalina to Sonoma), or a recent version of a Linux Distribution Operating System such that is capable of and you have administrative authorization to install software from third-party organizations (that is, not necessarily from an official store of these), and you can program with the Python 3.x. programming language under an IDE of your preference. What we mean with access is that you may connect through a data or wifi network to the Internet to a machine that has these requirements set, instead of physically bringing one of these to the workshop.

### Services
#### Google Account
The Google Earth Engine API is a cloud-service distributed by the company under Google Cloud, its umbrella suite for other public cloud services. To have access to them, it is necessary to have a Google account. Although you may already have one, we recommend setting another account for your software development endeavors if you intend to continue using and sharing projects under this service.
* _Click **[here](https://support.google.com/accounts/answer/27441?hl=en) to read the official documentation on how to set a Google Account (“For Myself”).**_

#### Google Cloud's (non-commercial) Google Earth Engine Project
Depending on your intentions, you may call Google Earth Engine’s API for either commercial or non-commercial uses. Since the objectives of this workshop are not to make a profit out of whatever we may produce from this cloud service, we will be using the non-commercial setting.
* _Click **[here]() to read our guide on how to set up and access your Google Cloud’s non-commercial Google Earth Engine project.**_
* _Click **[here](https://earthengine.google.com/noncommercial/) to read the official documentation regarding Google Cloud’s non-commercial usage of Google Earth Engine.**_

### Software
#### Python 3.11.6
The Google Earth Engine API is available for two programming languages: JavaScript, and Python. While the JavaScript API (under a non-commercial usage) is only available through the official web Code Editor, this workshop requires the usage of a local machine’s hardware capabilities; hence, the compulsory use of the Python 3.x programming language. Code written for this workshop has been done so with version 3.11.6.
* _Click **[here](https://www.python.org/downloads/release/python-3116/) to read the official documentation on how to install Python’s latest version (3.11.6). After downloading the corresponding installer (in the “Files” section), open and follow its instructions.**_

> [!WARNING]
> By the time we wrote these guides, Python 3.12 was released; this is its latest, so you may be prompted to either download or update your Python version to it. For this workshop, **do not install Python 3.12**, as we have detected errors in at least the installation of Google Cloud CLI for MacOS due to this version’s removal of used standard library packages. If you have it installed, remove it and download Python version 3.11.6.

> [!IMPORTANT]
> Your computer may have an already installed version of Python, usually 2.7.16; this is especially true if your computer runs MacOS or a Linux Distribution Operating System. After installing Python 3.11.6, to ensure that you are using Python 3.x. when calling ```python``` in a command line application, replace it with ```python3```.

### pip Package Manager
Having installed Python 3.11.6, we will require to install certain packages that are accessed through this programming language. For that, we will be using the pip package manager: Python’s main package distributor and installer. In this workshop, we are going to make use of its latest 23.3 version.
* _Click **[here](https://pip.pypa.io/en/stable/installation/#ensurepip) to read the official documentation on how to install pip’s latest version (23.3). We recommend you follow the ```ensurepip``` Supported Method for your Operating System. Follow the instructions right below the ```"ensurepip"``` header, written right above the ```get-pip.py``` option"**_

> [!WARNING]
> Your computer may have an already installed version of Python, usually 2.7.16; this especially true if your computer runs MacOS or a Linux Distribution Operating System. To ensure that pip is using Python 3.x when calling ```pip``` in a command line application, replace it with ```pip3```.

### Google Cloud CLI
Access to Earth Engine’s Python API requires the authorization of its usage by registering, retrieving, and authenticating your Google account credentials and Google Cloud projects. To store these on a local machine, you will require the installation of Google Cloud’s CLI. In installation, you will be prompted to log in with a Google Account: do so with the one you are using for your Google Cloud Earth Engine project under this workshop, and allow Google Cloud SDK access to your Google Account information. Then, return to your command line application and choose the Google Cloud project you have set up to use Earth Engine’s API.
* _Click **[here](https://cloud.google.com/sdk/docs/install) to read the official documentation on how to install Google Cloud’s CLI latest version for your Operating System and CPU architecture.**_

> [!WARNING]
> Follow our annotations on [Python 3.11.6](#python-3116). For this workshop, **do not install Python 3.12**, as we have detected at least Google Cloud CLI for MacOS installation errors under its usage.

> [!IMPORTANT]
> **For MacOS users:**
> For the purposes of this workshop, the official documentation’s Step 2.b.’s on how to install Google Cloud’s CLI for MacOS is **not optional**. Supposing that you already performed previous steps, and have extracted the contents of the `.tar.gz.` archive file in the Downloads folder, to ‘Run the script (from the root of the folder you extracted in the last step) [...],’ open the Terminal application, copy, paste, and run the following command:
> <br>
> ```
> cd Downloads
> ```
> Proceed to follow next steps.
> When asked `Modify profile to update your $PATH and enable bash completion? (Y/n)`, type and enter `Y`. After that, when asked to `Enter a path to an rc file to update, or leave blank to use [/Users/your_user/.bash_profile]:`, don’t write anything to leave blank, and press enter.
>
> Once installation has been completed, close and reopen your terminal.

### earthengine-api
Having installed the Google Cloud CLI, authorized and authenticated your Google account in its installation, and selected your Google Cloud Earth Engine project, we shall install Earth Engine's Python API using pip. On your terminal application, copy, paste, and run the `pip3 install earthengine-api --upgrade` command. Once the installation has finished, we will authenticate our Google account for Earth Engine's services usage: on your terminal application, copy, paste, and run the `earthengine authenticate` command; you will be redirected to log in or choose your Google account for Google Earth Engine's Authenticator, then allow it to access your Google account.

* _Click **[here](https://developers.google.com/earth-engine/guides/python_install) to read the official documentation on how to install Google Earth Engine's Python API `earthengine-api`, and authenticate your Google Account for Earth Engine's services usage.**_

### Visual Studio Code
Under this workshop, we will be using the latest version of Visual Studio Code IDE to walk-through, develop, and run the Python coding activities we have in store to aid us in the completion of our objectives. We have chosen this IDE as it widely supports the Python programming language through the installation and usage of Microsoft's official Python extension.
* _Click **[here](https://code.visualstudio.com/download) to read the official documentation on how to install Visual Studio Code for your Operating System and CPU architecture.**_

## Set-Ups
The following are standalone guides on specific set-ups we will be using for the development of the workshop’s materials. Following these is recommended both for the development and technical understanding of upcoming materials. If you decide to not use them, be mindful of the settings you have set as you read and progress through the workshop’s activities.

### Google Cloud’s (non-commercial) Google Earth Engine Project
* _Click **[here](./Set-Ups/Google%20Cloud’s%20(non-commercial)%20Google%20Earth%20Engine%20Project/README.md) to read our guide on how to set-up your Google Cloud's (non-commercial) Google Earth Engine Project for this workshop.**_

### Visual Studio Code extensions
Once Visual Studio has been installed, we will then make use of Microsoft's official extension for the Python programming language. Successful installation of this extension may require you to restart Visual Studio Code; close and reopen it.
* _Click **[here](https://marketplace.visualstudio.com/items?itemName=ms-python.python) to read the official documentation on how to install Microsoft's Python extension for Visual Studio Code.**_

## Testing your Set-Up
Having fulfilled aforementioned prerequisites, assumptions, and preferred set-ups, we will test our installations.
* To verify if you have Python 3.11.6 installed, open a command terminal application, and copy, paste, and run the following command (if necessary, change `python3` for `python`.) If correct, the command line should print `Python 3.11.6` after execution:
```
python3 --version
```

* Lastly, to verify if you have successfully installed Google Cloud CLI and earthengine-api under the right settings, open a command terminal application, and copy, paste, and run the following command (if necessary, change `python3` for `python`.) If both installations and set-ups are correct, the application should print `Successfully saved authorization token.` after execution:
```
python3 -c "import ee; ee.Initialize(project = '[yourname]-gaf23'); ee.Authenticate(auth_mode = 'appdefault');"
```
