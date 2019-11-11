# Pico Presentation
This is a repository of the Pico Presentation for FOAR705, 2019. This Pico Presentation outlines a Proof Of Concept Technology below for FOAR705,  2019.



# Managing Qualitative Data in the Field: Images, Metadata and Secure Storage

# Table of Contents
- [Background](#background)
- [Outline](#outline)
- [Requirements](#requirements)
- [Installation](#installation)
- [Testing](#testing)
- [Results](#results)
- [Limitations](#limitations)
- [Information](#information)


# Background:


This repository contains the Proof of Concept (POC) Technology Deployment for FOAR705, 2019. This POC contains an Automator workflow to export photos from Mac's default photo application into the research photo application Tropy, using ExifTool to embed additional metadata into the photos. Duplicati then securely backs up the work on a scheduled timer. This aims to demonstrate a more streamlined process for qualitative researchers in the field who want their photographic data to be more organised, detailed, managed and stored efficiently. 

# Outline:


This repository includes the Automation workflow, photos for testing, an exiftool script, a license and this README file. The following tools are implemented in this demonstration:

* **Automator** is an exclusive Mac application that programs a workflow by automating repetitive tasks using a drag and drop interface.

* **Tropy** is an open-source software program for research photo management.

* **Exiftool** is an open-source software program for reading, writing, and manipulating image, audio, video, and PDF metadata.

* **Duplicati** is an open-source software program thats stores securely encrypted backups on cloud storage services.

* **Github Desktop** is an open-source software program that seamlessly contributes to projects on Github and Github Enterprise. 

# Requirements:
This should only be run on a macOS Catalina, prior versions of macOS may not work. It cannot be run on Windows.

This demonstration needs the application Automator. This is a default application in macOS Catalina and is required.

This demonstration needs the application Photos. This is a default application in macOS Catalina and is required.

The application Tropy needs to be downloaded from [Tropy.org](https://tropy.org/download/mac)

The software program ExifTool needs to be downloaded from [ExifTool](https://www.sno.phy.queensu.ca/~phil/exiftool/ExifTool-11.75.dmg)

The application Duplicati can be downloaded from [Duplicati](https://updates.duplicati.com/beta/duplicati-2.0.4.23_beta_2019-07-14.dmg)


The application Github Desktop needs to be downloaded from [Github](https://central.github.com/deployments/desktop/desktop/latest/darwin)

The application Automator can be viewed in more detail in the [Automator User Guide](https://support.apple.com/en-au/guide/automator/welcome/mac)

The application Photos can be viewed in more detail in the [Mac Photos User Guide](https://support.apple.com/en-au/HT206186)

* Note: Duplicati is not involved in this installation and test, as its has been demonstrated in an FOAOR705 consultation. To use Duplicati, download from the link above and schedule a daily backup on the projects location after tests have been run.

* Note: Github Desktop requires a user account to access these tools. Sign in or create an account to continue with this POC demonstration. 



# Installation:


* Ensure you have met the requirements in the section above before proceeding.
* Download and install Tropy, ExifTool and Github Desktop from the links above.
* Clone this repository to your computer via Github Desktop. 
* It is important that the file Exiftool_Script is in folder ~/Documents/GitHub/SophieWallace_POC_Contents/
* Create an album named "Export" in default Mac Photos application.
* Move the test images from this repository into the newly created "Export" folder in Mac Photos application.



# Testing:


* Open POC_Workflow_DEMO in the application Automator.
* Once POC_Workflow_DEMO is open, select run in the top right corner of Automator.
* Prompt for writing location should appear.
* Write location metadata for the photos, in this case "Changu Narayan".
* Tropy interface appears and tropy_input images appear in finder window.
* Create Tropy project.
* Drag photos from tropy_input folder into Tropy.


# Results:


* Exported images are now in a folder on the desktop named tropy_input, with the current date and time.
* Images in the folder are now named Nepal, with the current date and time.
* Once dragged into Tropy, images have 'creator' metadata named Sophie Wallace.
* Once dragged into Tropy, images have 'date' metadata, with the original date and time of photo.
* Once dragged into Tropy, images have aribitrary 'type' metadata written from the prompt asking for geo-location.




# Limitations:

This POC technology deployment has limitations. Instructions for using these applications to their full potential are not included in this package. These programs are wide-ranging and specific to each user. Therefore, instructions on the overall usage of these applications are too extensive to include. To mitigate this, I have provided links below in 'further information'. The Automator link for additional detail is above in requirements.

In the initial scoping, elaboration and user stories for this POC, the tool described organised diverse data-sets. Due to time constraints and limited resources, this POC technology only works for image data. Despite this, most user stories have been accomplished.

This POC technology deployment is only available on macOS catalina. This is a significant limitation for users with a different operating system. Due to the scope of this POC, solving this pain was unattainable. 

This POC technology deployment has specific limitations with Automator and Tropy. Additionally, there are some anticipated errors that occur in this demonstration. Limitations and errors below:


**Automator**
* Utilising key commands such as "command A" crashed the application.
* The 'Watch Me Do' action responds slowly.
* Actions such as renaming folders, work haphazardly.
* Actions are extremely limited.
* Actions focus predominantely on Mac applications.
* Only available on macOS Catalina.

**Tropy**
* Tropy does not work with the command line
* Tropy does not accept different data types
* Tropy does not work with Mac default photos application

**ExifTool**
* After downloading, ExifTool may not open succesfully.
* Open with terminal and then double click on the package again.
* If this fails, visit ExifTool link below for more information.

**Duplicati**
* After downloading, Duplicati may not open successfully.
* If this occurs, download Duplicati directly from this website [https://www.duplicati.com/download](https://www.duplicati.com/download)

# Information:

For more information on Tropy visit [https://tropy.org/](https://tropy.org/) 

For more information of ExifTool visit [https://www.sno.phy.queensu.ca/~phil/exiftool/](https://www.sno.phy.queensu.ca/~phil/exiftool/)

For more information on Duplicati visit [https://www.duplicati.com/](https://www.duplicati.com/)

For more information on Github Desktop visit [https://desktop.github.com/](https://desktop.github.com/)

