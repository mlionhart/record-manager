# CTEC 127 - Project No. 4

## Project Overview

Be sure to clone this repository to your computer before reading any future. Place it in your **htdocs** folder.

This project will have you modify your code from Project No. 3 of the **Record Management** application and have you add **Update** functionality to it. I also want you to include the revised functionality to properly show the last name filtering. Read on for more info on this.

Your entire Project No. 3 will need to be modified once you are done with it to include Updating functionality.

I have provided all of the resources that you will need to make these changes.

This code base is a revision to my Project No. 3 Starter Code.

See Canvas for the due date.

Here are the items that have changed:

- The **form.inc.php** code has been moved from the **create** folder to a new folder named **shared**.
- A new folder named **update** has been added which contains **content.inc.php**.
- The function named **display_record_table** has been modified to include new code to support updating.
- The **form.inc.php** file has been modified to include a new hidden field. This field stores the **id** (primary key) of the student record.
- The **update-record.php** file has been modified to include support for updating records. Prior to this this file had placeholder text only.
- The function **display_record_table** to display the filtering now works when the page is resized.
- All of the PHP **require** statements have been to changed to require_once.
- The inclusion of **functions.inc.php** has been moved into the **header.inc.php** file.
- The navigation bar now highlights the active page in the navigation.
- A new **echoActiveClassIfRequestMatches** function has been added to functions.inc.php. You can see it action in the **navbar.inc.php** file.

There are no changes to the database that you will need to make for this project.

## File and Folder Structure

- css
  - bootstrap.min.css
  - style.css
- img
  - frown.png
  - nosmile.png
- inc
  - app
    - config.inc.php
  - create
    - content.inc.php
  - db
    - mysqli_connect.inc.php
  - display
    - content.inc.php
  - functions
    - functions.inc.php
  - layout
    - footer.inc.php
    - header.inc.php
    - navbar.inc.php
  - shared
    - form.inc.php
  - update
    - content.inc.php
- js
  - bootstrap.min.js
  - query-3.3.1.min.js
- sql
  - student_v2.sql
- create-record.php
- delete-record.php
- display-records.php
- search-records.php
- update-record.php

## Application Overview

The **Record Management** application has 4 pages that are used by end users.

- **display-records.php** - This is the page that should be launched to start within the applicaiton
- **create-record.php** - This page is used to create new records that get inserted into the database
- **search-records.php** - This page gets called when somebody enters text in the navigation bar search box and clicks on the **Search** button.
- **update-records.php** - This page gets called when somebody clicks on the **Update** link next to a record.

All of these pages uses various components from the **inc**, **css**, **img**, **functions**, **layout**, **app**, **create**, **db**, and **js** folders.

The folders for **css**, **img** and **js** are self explanatory.

The **db** folder is used for the **mysqli_connect.inc.php** that allows the entire application to connect to the **MySQL (MariaDB)** database.

The **inc** folders and **subfolders** have the following sub-folders:

- **app** is used to store a PHP file that stores variables that are used throughout the application.
- **create** contains the files that are included in the **create-record.php** page.
- **display** contains a file that gets included in the **display-records.php** page.
- **functions** contains a file that has several functions that are used throughout the application.
- **layout** contains the files for page layout such as the **header**, **footer** and top **navigation**.
- **update** contains a file that gets included in the **update-record.php** page.
- **shared** contains a file that has the code for the create/update form.