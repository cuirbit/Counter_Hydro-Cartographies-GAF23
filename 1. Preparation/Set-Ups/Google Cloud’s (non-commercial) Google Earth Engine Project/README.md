# Google Cloud's (non-commercial) Google Earth Engine Project
> [!NOTE]
> _**The following guide is part of the Counter Hydro-Cartographies workshop under the Gray Area Festival 2023: Plural Prototypes and the C/Change Initiative.**_ _**Click [here](../.../../../) to go to the workshop’s main github page.**_

> [!IMPORTANT]
> We remind readers of these guides that they were written for a workshop taken in late 2023; by the time you read them, these might be outdated.

> [!WARNING]
> Access to Google Cloud services requires a Google account. While this may be your personal @gmail account, we recommend you sign up another one for the purposes of your own development efforts.
> * _Click **[here](https://support.google.com/accounts/answer/27441?hl=en) to read the official documentation on how to set a Google Account (“For Myself”).**_

<br>
The following guide walks you through the creation of a non-commercial (‘Unpaid usage’) Google Cloud project. Its registration’s details have been filled in relation to the workshop it is used on.

## Google Earth Engine's Webpage
Open a browser. Then, go to [Google Earth Engine’s home site](https://earthengine.google.com/). You should see the following webpage.
<br>
<br>
![Screenshot of Google Earth Engine’s home site.](./0.%20Assets/GoogleEarthEngine_webpage.png)
<br>
<br>
## Google Cloud Project Registration
### Get Started using Earth Engine
Located in the site’s right top corner, click the [‘Get Started’](https://code.earthengine.google.com/register) button. If you haven't logged in into your Google account previously, you will be asked to do so. If you have logged in with more than one Google account, you may be redirected to a page asking to choose which account to use; if it doesn’t, you may consider switching your account by clicking on your profile picture located at the site’s right top corner, and then clicking ‘Switch Account’. Having completed that prerequisite, you will be redirected to the following page.
<br>
<br>
![Screenshot of Google Earth Engine’s site to register an Earth Engine project](./0.%20Assets/RegisterEarthEngineProject_webpage.png)
<br>
<br>
### How do you want to use Earth Engine?
If you already have a project, you may click the [‘Click here to go to the Code Editor’](https://code.earthengine.google.com/) hyperlink located in the bottom side of the page. While you can sign non commercially your account up to use Earth Engine noncommercially (under the ‘Click here for the signup form’ hyperlink] without the need of a project’s creation, approval to use may take a few days to be given. For our purposes, we are to register a Google Cloud project: click the ‘Register a Noncommercial or Commercial Cloud project’ button at the center of the page. You should see the following options.
<br>
<br>
![Screenshot of Google Earth Engine’s site to register an Earth Engine project displaying a form asking under which usage an user has intentions of for the creation of a new Google Cloud project. Two mutually exclusive options are displayed: ‘Paid usage’, and ‘Unpaid usage.’](./0.%20Assets/HowDoYouWantToUseEarthEngine_webpage.png)
<br>
<br>
The site erases its previous options to display two mutually exclusive buttons in which you will select how you want to use your new Earth Engine project: ‘Paid usage’ or ‘Unpaid usage’. For the purposes of this workshop, choose ‘Unpaid usage’. After doing so, a ‘Project type*’ selector displays under the ‘Unpaid usage’ option; click it, and choose ‘No affiliation.’ Your form should look like the following image. If true, click the ‘Next’ blue button.
<br>
<br>
![Screenshot of Google Earth Engine’s site to register an Earth Engine project displaying a filled form asking under which usage an user has intentions of for the creation of a new Google Cloud project. Two mutually exclusive options are displayed: ‘Paid usage’, and ‘Unpaid usage.’ The latter option is selected. A ‘Project type*’ selector displays under this option; ‘No affiliation’ is chosen.](./0.%20Assets/HowDoYouWantToUseEarthEngine_webpage_filled.png)
<br>
<br>
### Create or choose a Cloud Project to Register
Once again, the site erases its previous options to display another two mutually exclusive buttons in which you will select to ‘Create a new Google Cloud Project’ or ‘Choose an existing Google Cloud project.’ The site should look like this.
<br>
<br>
![Screenshot of Google Earth Engine’s site to register an Earth Engine project displaying a form asking whether to create or choose a Cloud Project to register. Two mutually exclusive options are displayed: ‘Create a new Google Cloud Project’ or ‘Choose an existing Google Cloud project.’](./0.%20Assets/CreateOrChooseACloudProjectToRegister_webpage.png)
<br>
<br>
Choose the ‘Create a new Google Cloud Project’ option. After doing so, a new part of the form displays. For this workshop: in the ‘Organization’ selector, choose ‘No organization’; in the ‘Project-ID*’ text box, write your name followed by ‘-gaf23’; in the ‘Project Name (optional)’ textbox, write your name followed by -‘ GAF23.’  The form should look similar to this. If so, click the ‘Continue to Summary’ blue button.
<br>
<br>
![Screenshot of Google Earth Engine’s site to register an Earth Engine project displaying a form asking whether to create or choose a Cloud Project to register. Two mutually exclusive options are displayed: ‘Create a new Google Cloud Project’ or ‘Choose an existing Google Cloud project.’ After having chosen ‘Create a new Google Cloud Project, a new set of options is displayed: in the ‘Organization’ selector, the ‘No organization’ option is chosen; in the ‘Project-ID*’ textbox, ‘yourname-gaf23’ has been written; in the ‘Project Name (optional)’ textbox, ‘yourname - GAF23’ has too.](./0.%20Assets/CreateOrChooseACloudProjectToRegister_webpage_filled.png)
<br>
<br>
### Confirm your Cloud Project Information
You will be redirected to a new page displaying a summary of your new Google Cloud project’s filled characteristics. As stated in the page, ‘Project information cannot be changed later’; in the case that you would like to edit a detail before finally registering your project, for each one of them, there is a pencil-icon button which allows you to edit such information. After revising that the information you have provided is correct, this page should look similar to this. Click the ‘Confirm’ blue button.
<br>
<br>
![Screenshot of Google Earth Engine’s site to register an Earth Engine project displaying a new project’s user-filled details before confirming the registration process. In ‘Project usage’, the ‘No affiliation’ option is seen as chosen; in ‘Project info’, ‘yourname-gaf23’ and ‘yourname GAF23’ are shown as having been written.](./0.%20Assets/ConfirmYourCloudProjectInformation_webpage.png)
<br>
<br>
## Google Earth Engine's Code Editor
After confirming registration details, it will be submitted. Having completed the registration, you will be redirected to Google Earth Engine’s Code Editor. Here, Earth Engine’s API is available for the Javascript programming language. In this workshop, we will be using Python’s.
<br>
<br>
![Screenshot of Google Earth Engine’s Code Editor. It has been opened for the ‘yourname-gaf23’ project.](./0.%20Assets/GoogleEarthEngineCodeEditor_webpage.png)
<br>
<br>
