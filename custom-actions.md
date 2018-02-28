# SeedCode Custom Action Style Guide (Ever Evolving)

## Table of Contents

  1. [Overview](#overview)
  1. [Header](#header)
  1. [Comments](#comments)
  1. [Variables](#variables)
  1. [Links](#links)

## Overview
  
  - **Objective**
  This style guide is intended to ensure that custom actions developed for DayBack Online meet standards
  
  - **Freestanding**
  The code should stand on it’s own: Anyone should be able to get the custom action to work without having to ask too many questions or refer to too many other pieces of knowledge.
  The function is self-contained.
  
  - **Egalitarian**
  The code should be understandable and editable by anyone who looks at it.
  It should be hospitable and welcoming to people who implement it into their DayBack instance, as well as those who come across it at a later time.
  There should be links from the docs on any DayBack functions used.
  Avoid using jargon in the comments.
  

## Header
  
  - **Title and version number**
  The header should start with a title of the custom action and the current version number.  
  
  - **Description of function**
  Below the title, enter a description in laymans terms, that explains exactly what the function accomplishes. This should contain a Purpose, Action Type, and Link to docs.
  
  
  ###### Example 1:
  
    //Validate Field Entry v1.2
  
    //Purpose:
    //This function will send an email to support with the following details:
    //Email To - support@seedcode.com
    //Subject - Event Title
    //Body - Event description
  
    //Action Type: Custom Action
    //Open in new window: no
  
    //More info on custom actions here:
    //https://www.seedcode.com/pmwiki/index.php?n=DayBackOnline.CustomActions
  
  
  ###### Example 2:

    //Validate Field Entry v1.2

    //Purpose:
    //Verifies that specified additional fields have a value entered
    //Prevents saving the event if the specified additional field's value is empty

    //Action Type: Before Event Save
    //Prevent Default Action: Yes

    //More info on Before Event Save actions and objects here:
    //https://www.seedcode.com/pmwiki/index.php?n=DayBackOnline.CustomActionObjects#BeforeSave

**[⬆ back to top](#table-of-contents)**

## Comments

  Comments should explain the purpose of each function, as well as the variables used and which ones should be modified.
  
  - **User editable section**
  
  Anything that needs to be edited by the user should be set in variables at the top of the main function.
  
  - **Do Not Edit notification**
  
  All code that should not need to be edited by the user should be clearly marked with the following comment:
  //----------- You shouldn’t need to edit below this line -------------------
  
  Anything after that line should not need to be edited by the user


**[⬆ back to top](#table-of-contents)**


## Variables

  Variables that may need to be edited by the user should be declared at the top of the main function in their own commented section
  
  After declaring user editable variables, declare any additional necessary variables below the "Do Not Edit" notification.
  

**[⬆ back to top](#table-of-contents)**


## Links

  All DayBack functions used in the custom action should have comments referring to links in the docs that describe the function.


**[⬆ back to top](#table-of-contents)**
