---
permalink: /institutional-customization-guide/
title: "Institutional Customization Guide"
excerpt: "DMP Assistant Institutional Customization Guide"
date: 2022-04-25
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/big.jpeg
  actions:
    - label: "Use DMP Assistant"
      url: "https://assistant.portagenetwork.ca"
toc: true
toc_label: "Institutional Customization Guide"
toc_icon: "cog"
---
DMP Assistant Institutional Customization Guide
===============================================

### _Version 1.0, July 13, 2016 – currently being updated_

Acknowledgements
----------------

Thanks to all members of the Portage DMP Customization Working Group for their contributions to this guide. Members are: Jay Brodeur (McMaster University), Talia Chung (University of Ottawa), Carla Graebner (Simon Fraser University), Alex Guindon (Concordia University), Amber Leahey (Scholars Portal), Anthony Petryk (University of Ottawa), and Weiwei Shi (University of Alberta). Special thanks are expressed to all institutions and individuals who assisted with testing and revision of this document.

Introduction
------------

The purpose of this document is to instruct local administrators of the modifications that can be made to [DMP Assistant](https://assistant.portagenetwork.ca), in order to customize its content and appearance to meet their local institutional needs. The following guide introduces the organizational administrative interface, and demonstrates how it can be used to modify DMP Assistant templates (questions and guidance), as well as the “look and feel” of the GUI.

This document was produced by members of the [Portage Data Management Planning Expert Group](https://portagenetwork.ca/about/network-of-expertise/expert-groups-membership/#DMPEG).

[![PDF icon](https://portagenetwork.ca/wp-content/uploads/2016/07/Adobe_PDF_file_icon_32x32.png)](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPAsssistant_Customization_Guide_1.0_EN.pdf) You may also download this guide [in PDF format](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPAsssistant_Customization_Guide_1.0_EN.pdf).

### Contents

[1 Preparing for customization](#section1)  
[2 Accessing and using the organizational administrative interface](#section2)  
[2.1 Accessing the organizational administration interface](#section21)  
[2.2 Editing organization details](#section22)  
[3 Customizing institutional logos, banners and color schemes](#section3)  
[3.1 Preparing logo and banner images](#section31)  
[3.2 Uploading images to DMP Assistant](#section32)  
[3.3 Special notes on interface customization](#section33)  
[4 GUI CSS customization](#section4)  
[4.1 Overview](#section41)  
[4.2 Example: Institutional CSS customization](#section42)  
[4.2.1 Institutional hexadecimal colour codes](#section421)  
[4.2.2 Section heading colour](#section422)  
[4.2.3 Footer colour](#section423)  
[4.2.4 Top banner text colour](#section424)  
[4.2.5 Colour of buttons and tables](#section425)  
[4.2.6 Tab colour](#section426)  
[4.2.7 Question section colour](#section427)  
[4.2.8 Guidance and suggestion box colours](#section428)  
[4.2.9 Top banner background color](#section429)  
[5 Template customization and management  
](#section5)[5.1 Template management](#section51)  
[5.1.1 Template](#section511)  
[5.1.2 Phase and version](#section512)  
[5.1.3 Sections and questions](#section513)  
[5.1.4 Publishing](#section514)  
[5.2 Adding additional institutional guidance text](#section52)  
[5.2.1 Previewing institution specific guidance](#section521)  
[5.2.2 Using institution specific guidance](#section522)  
[6 Reporting issues/bugs and suggesting new features](#section6)

1\. Preparing for customization
-------------------------------

To get started with customizing DMP Assistant for your local institution, you will need the following:

*   An institutional space within DMP Assistant. This can be requested from the Portage Network by contacting [portage@carl-abrc.ca](mailto:portage@carl-abrc.ca). With an institutional space, a local administrator will have administrative rights to edit basic organizational information and to implement some local customization options. It is recommended that a generic user account be used for administration, as it will reduce the possibility of accidentally transferring administrative privileges between user accounts;
*   An individual designated as your institution’s DMP Assistant local administrator;
*   Your institution’s logo image with a maximum height of 80 px;
*   A CSS file based on the current [template](https://github.com/ualbertalib/DMPonline_v4/blob/deployment-portage/app/assets/stylesheets/umcmaster-custom.css) and modified according to the instructions provided in Section 2;
*   The hexadecimal colour codes for branding colours commonly used by your institution (to be used in the CSS file); and,
*   (\*Optional\*) A top banner image with a height between 90 px to 160 px ([example](https://raw.githubusercontent.com/ualbertalib/DMPonline_v4/deployment-portage/app/assets/images/top_back.png))

For management and accessibility reasons, we ask that you only customize the elements that are described in this guide, using the provided methods. In the case that additional customization is desired, please contact [portage@carl-abrc.ca](mailto:portage@carl-abrc.ca).

2\. Accessing and using the organizational administrative interface
-------------------------------------------------------------------

As an organization’s local administrator, you can log in and use the organization admin interface to manage your institutional space.

Once you have entered the organizational administrative interface, you will be able to:

1.  Edit organization details;
2.  View basic information for users associated with your organization (email address, last time of log-in, and the number of plans they have created);
3.  Create, edit, manage and delete organization specific templates; and,
4.  Create, edit, manage and delete organization specific guidance.

### 2.1 Accessing the organizational administration interface

Once logged into DMP Assistant with your administrator account, click on **Signed in as …** and then select **Admin area** to access the organizational administration interface.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_1.png)

Figure 1: Click on Admin area to access the organizational administration interface.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_2.png)

Figure 2: The organizational administrative interface.

### 2.2 Editing organization details

As the local administrator, you may view and edit the information for your organization. Please note, for the time being, not all features are enabled. To edit organizational details:

Click on **Organization details** to view your organization’s basic profile information.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_3.png)

Figure 3: Click on Organization details to view your organization’s basic details

Click on the **Edit** button to edit the organization details.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_4.png)

Figure 4: Click on the Edit button to edit the organization details.

In the editable organization details page, local administrators can modify their organization’s name, abbreviation, website URL, descriptive information, as well as upload an institutional logo, top banner image, and customized CSS file (see following sections).

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_5.png)

Figure 5: The editable organizational details page

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_6.png)

Figure 6: Editing organizational details.

3\. Customizing institutional logos, banners and color schemes
--------------------------------------------------------------

To create a local “look and feel” for DMP Assistant users logged-in with their particular institution, local administrators can modify one (or all) of the following elements: institutional logo; top banner image/color; and, institutional-specific color schemes (see Figure 7). The following guidance outlines these customization processes:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_7.png)

Figure 7: An example of a fully-customized DMP Assistant interface.

### 3.1 Preparing logo and banner images

For optimal presentation, your selected institutional/organizational logo image should have a maximum height of 80 px.

The use of a top banner background image ([example](https://raw.githubusercontent.com/ualbertalib/DMPonline_v4/deployment-portage/app/assets/images/top_back.png)) is optional. If you choose to use one, the image should have a height between 90 and 160 px for optimal presentation. Alternatively, you can forego the use of a banner image and instead customize the page CSS to select a solid background color for the banner area (see Section 2).

### 3.2 Uploading images to DMP Assistant

To upload the images, follow the steps below:

1.  Login as administrator and follow the steps outlined in Section 1 to access the editable organization details page.
2.  Prepare logo and banner images (instructions); customize your CSS file (instructions).
3.  Use the interface to upload your customized logo, banner and CSS files into the administrative interface.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_8.png)

Figure 8: Use the organizational details interface to upload customized logo, banner and CSS files.

### 3.3 Special notes on interface customization

For technical and administrative purposes, administrators should not modify the CSS code beyond that which is demonstrated in the following section (GUI CSS customization).

Other small changes may be possible on a case-by-case basis. If you require specific changes, please contact [portage@carl-abrc.ca](mailto:portage@carl-abrc.ca).

If a new image or CSS file is uploaded, the existing files will be overwritten. If you decide to switch back to original Portage logo/stylesheet and remove all customizations, please follow the directions on the interface. Check the checkboxes and click on **Save** to remove uploaded images, and click on the deletion link to remove uploaded CSS file.

4\. GUI CSS customization
-------------------------

### 4.1 Overview

Using [McMaster University’s customized CSS file](https://github.com/ualbertalib/DMPonline_v4/blob/deployment-portage/app/assets/stylesheets/umcmaster-custom.css) as a template, institutions can customize the colour scheme of DMP Assistant page using the CSS hexadecimal scheme. The thoroughly commented CSS template (providing additional annotations for each of the allowed colour changes) can be accessed and downloaded [here](https://github.com/ualbertalib/DMPonline_v4/blob/deployment-portage/app/assets/stylesheets/umcmaster-custom.css).

Before you begin editing the CSS file, you will need the hexadecimal colour codes commonly used by your institution. These begin with a # symbol and are followed by six characters (numbers and/or letters). For example, white is #FFFFFF (or #FFF for short) and light grey is #333333.

Once you have your institution’s colours, you can open the CSS template in a text editor (such as Notepad++) and start replacing the existing colours with your institution’s colours.

To ensure you’re using the correct hexadecimal colour scheme, you can use something like [www.color-hex.com](http://www.color-hex.com) to verify.

Before you upload your revised CSS to DMP Assistant, ensure you have saved your file with the .css extension.

### 4.2 Example: Institutional CSS customization

The following example illustrates and documents the customization process, as applied by a single institution (McMaster University in this case). Screenshots were taken to show modifications made to the CSS code (with line numbers included, for easy reference), as well as the resulting changes to the interface. Each modification is presented in a separate section; screenshots of editable sections of the CSS file are shown first, followed by the resulting changes to the GUI. Please note that each modification has been applied independently, in order to better demonstrate the resulting effects.

#### 4.2.1 Institutional hexadecimal colour codes

For the purposes of this example, McMaster’s hexadecimal colour codes were found by consulting its [branding guide](http://www.mcmaster.ca/opr/html/opr/mcmaster_brand/main/mcmaster_brand.html). The codes are as follows:

*   #79133E-maroon
*   #fff-white
*   #990033-red

#### 4.2.2 Section heading colour

Replace the hex colour code (#79133E) in the CSS snipped shown below with a desired colour.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_9.png)

Figure 9: Section heading changes in the CSS file.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_10.png)

Figure 10: Resulting section heading colour changes in the GUI.

#### 4.2.3 Footer colour

Modify the hex colour codes for the footer banner (6 character hex code) and the footer text colour (3 character hex code).

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_11.png)

Figure 11: Footer colour changes in the CSS file.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_12.png)

Figure 12: Resulting footer colour changes in the GUI.

#### 4.2.4 Top banner text colour

Modify the hex colour code for the three lines shown below

![](https://portagenetwork.ca/wp-content/uploads/2016/07/figure13.png)

Figure 13: CSS file changes for the top banner colour (3 steps).

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_16.png)

Figure 14: Resulting footer colour changes in the GUI.

#### 4.2.5 Colour of buttons and tables

Modify the hex colour code for the four lines shown below:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/Figure15.png)

Figure 15: CSS file changes for the button and table colours (4 steps).

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_21.png)

Figure 16: Resulting table and button colour changes in the GUI.

#### 4.2.6 Tab colour

Modify the hex colour code in the three lines shown below:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_22.png)

Figure 17: CSS file changes for tab colour.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_23.png)

Figure 18: Resulting tab colour changes in the GUI.

#### 4.2.7 Question section colour

Modify the hex colour codes for the four lines shown below:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_24.png)

Figure 19: CSS file changes for section colour.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_25.png)

Figure 20: Resulting section colour changes in the GUI.

#### 4.2.8 Guidance and suggestion box colours

Modify the hex colour codes for the three lines shown below:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_26.png)

Figure 21: CSS file changes for guidance and suggestion box colours.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_27.png)

Figure 22: Resulting guidance and suggestion box colour changes in the GUI.

#### 4.2.9 Top banner background color

To use a customized background color, add the following line to your CSS (replacing #c7e2fa with a hex colour code of your preference).

     .dmponline {
           background-color: #c7e2fa;
           }

5\. Template customization and management
-----------------------------------------

The Portage template can be regarded as a generic DMP template that can be used “out of the box” by any researcher. Not all institutions will need nor want to develop an institutional template, but the functionality is available for those who feel it is important for their organization. For those institutions wishing to provide customized templates (questions and guidance) to meet specific needs, the following steps demonstrate how a custom template can be created using the administrative interface.

### 5.1 Template management

The steps for template management follow the logical sequence of Template->Phase->Version->Section->Questions. Please note that at any point, you can preview the template by clicking on **Preview** under **Actions**.

#### 5.1.1 Template

To create a new template, click on Templates on the top navigation, and then click on **Create a template**:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_28.png)

Figure 23: The Templates page allows you to view, edit or create new templates.

Provide title and description information for the new template, and then click on **Save**:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_29.png)

Figure 24: Inserting title and description for a new template.

#### 5.1.2 Phase and version

Phases are used to indicate different stages of a research project (e.g. pre- / during / post-project). The generic Portage Template is not a phased template. To create a single phased template like the generic Portage Template, you only need to add a new phase once. Click on the Add new phase+ tab to add a new phase of the template. The phase title is what users will see in the tabs when completing a plan. If you only need one phase, you may wish to give it a generic title such as _<Your Institution>\_ Data Management Questions_.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_30.png)

Figure 25: Adding a phase to a template.

When a new phase is created, the creation of a new version of the template is triggered. For example, when the new phase is created for a new template, the first version of the template will be automatically created.

To make major changes to a template that has already been published (such as adding a new section or series of questions), you should create a new version. To make small changes such as correcting typos, choose to edit the current version.

Click on **Save** to move on to creating sections and questions.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_31.png)

Figure 26: The template details page.

#### 5.1.3 Sections and questions

To add a new section, enter the section title at the bottom of the _Version editing_ page, and click on **Add section**. Use the **+** to expand the section editing window for adding description information and to define the order in which the sections will be displayed.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_32.png)

Figure 27: Adding a new section.

Add questions to each section by selecting **Add question**.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_33.png)

Figure 28: Adding a new question.

When adding questions, you can:

*   Use the Question number dropdown menu to define the display order of questions within a section: eg. Question number 1 will be displayed first in the section. By changing the question number, the order in which the questions appear on the template will change accordingly.
*   Choose the _Answer format_:
    *   _text area_ for long paragraphs of text;
    *   _text field_ for a short text answer;
    *   _checkbox_ for presenting options for multiple value selection;
    *   _radio button_ for presenting options for single value selection;
    *   _dropdown list_ for controlled vocabulary selection;
    *   _multiple select box_ for allowing users to select multiple options from a scrollable list using the CTRL key.
*   Define _default answer_ for each question. The answer will be displayed in the answer box for users.
*   Define a _suggested answer_ for each question. The example provided will be presented above the answer box and can be easily copied/pasted by the user.
*   Create question specific _guidance_. The guidance text entered here will always be displayed alongside the question, no matter what other guidance groups are selected (guidance groups are described in section 3.2.1).

#### 5.1.4 Publishing

Once the sections and questions have been created, select the _Published_ checkbox in the _Version_ editing section to indicate the active version being used within your template. This step is necessary and indicates that the version is active and ready to be published as part of a template which itself must be published before it is made public.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_34.png)

Figure 29: “Publish a version”, the checkbox is selected, then save to publish the template.

Once a version has been marked as published, return to the Template details tab. Select **Edit template details**.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_35.png)

Figure 30: “Template details” tab to access the template details editing page. Remember to first select a version of the template before proceeding to publish.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_36.png)

Figure 31: “Template details editing” page with the checkbox selected in order to publish the template.

Once the template is published, your users will see your new template as an available selection when they create a new DMP. The institutional template will be the default template and will be listed first in the dropdown selection menu.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_37.png)

Figure 32: “Create a new plan” page showing two published templates as options.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_38.png)

Figure 33: Confirmation dialogue box showing selection of customized institutional template.

#### 5.2 Adding additional institutional guidance text

In some cases, it may be desirable or necessary to enhance a template’s existing guidance text (e.g., the Portage template guidance) with additional, institutional-specific instructions.

In order to create institution-specific guidance text, local administrators must first create one or more Guidance Groups, to which guidance texts can be associated. Once this is done, the local administrator can generate an institutional guidance frame, which appears alongside the default template guidance in the GUI, by creating a guidance group guidance text.

1.  You will need to first create a Guidance Group for your institution

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_39.png)

Figure 34: Guidance group list, allowing the creation of new guidance groups and guidance text.

*   You can identify which templates should be associated with a particular guidance group. You could create Portage and institution specific guidance as needed or generic guidance text that is applicable to all templates for users from your institution.
*   If the guidance is only meant for a subset of your users, you can save the guidance as an optional subset. Users will be able to select whether or not to display this subset in the create plan wizard.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_40.png)

Figure 35: Assigning a guidance group to a template.

2.  Once the guidance group is created, create individual guidance text by selecting Add guidance. You can draft guidance language to accompany specific questions.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_41.png)

Figure 36: Creating new guidance text.

*   For guidance by question, you will need to indicate:
    1.  the template in which the question is found;
    2.  the phase of the template (e.g. phase for early vs. late part of the data management process);
    3.  the version of the template;
    4.  the section from the template in which the question is found; and,
    5.  the question to which the guidance will apply.

#### 5.2.1 Previewing institution specific guidance

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_42.png)

Figure 37: Click Preview to preview institutional specific guidance.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_43.png)

Figure 38: A preview of institutional guidance.

#### 5.2.2 Using institution specific guidance

1.  On the create plan page, select your institution from the drop down menu.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_44.png)

Figure 39: Selecting an institution when creating a new plan.

2.  Next, select the template to which the guidance applies.

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_45.png)

Figure 40: Selecting a template when creating a new plan.

3.  Last, select the institution-specific guidance you wish to display (if it has been listed as an optional subset).

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_46.png)

Figure 41: Enabling additional guidance sources when creating a new plan.

It looks like this in the user interface:

![](https://portagenetwork.ca/wp-content/uploads/2016/07/DMPcustom_47.png)

Figure 42: Example of institutional-specific guidance during normal use.

6\. Reporting issues/bugs and suggesting new features
-----------------------------------------------------

All issues, bugs and new feature requests can be submitted via the issues page on DMP Assistant’s GitHub page: [https://github.com/ualbertalib/DMPonline\_v4/issues](https://github.com/ualbertalib/DMPonline_v4/issues). In order to submit issues to the Github page, you must first have a Github user account (can be created at no cost).