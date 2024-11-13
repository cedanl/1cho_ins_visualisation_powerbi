# 1cho_ins_visualisation_powerbi
Each Higher Education institution receives the 1cHO_inschrijvingen_instellings_bestand once a year. This file contains data regarding the registrations of all their current students. The files in this package contain a fully working powerBI dashboard ready to run on the 1cHO_inschrijvingen_instellings_bestand and all accompanying supportfiles without the need for any further data transformations on these files.

PowerBi consists of a visualisation part and a data transformation part (powerquery). For this dashboard to run there is no need to tinker with the powerquery part. Any adjustments that might be needed for the powerqueries to run proparly can be made in the data visualisation part of powerBI through parameters (explained below). However, in order to get the full experience and possibilities of powerBI powerquery knowledge is a must.

# More information
In this README the first usage of this package is explained. However, for more in depth information on how to use the package and the underlying data files please check the wiki: https://github.com/ed2c/1cho_ins_visualisation_powerbi/wiki

# Installation
A prerequisite for running this package is being able to run powerBI, either the online version or the desktop version. It is highly recommended to use the desktop version. However, you can also use the online version during the demo. You will miss out on some functionalities though. The desktop version lets you tinker with the powerqueries and the parameters while the online version does not.

For both options you will need to download or pull the raw file 1cHO inschrijvingen instelling.pbix, NPuls Theme aanpas.json, the header_files, the supporting_files, and the input.

### How to install the desktop version:
You will need to download and install powerBI. A free to use download can be found here: https://powerbi.microsoft.com/en-us/downloads/. The desktop version of powerBI is free to use. However, if you want to publish the dashboard to the rest of your organisation a powerBI pro or premium license is needed.

### How to install the online version:
The prerequisite for this option is that your organisation as some sort of microsoft licence. If your organisation uses microsoft teams, this should be in order. Go to https://app.powerbi.com and log in with your organisation's email account. Once you have logged in you can open your personal workspace (located in the left menu).

<img width="55" alt="My workspace" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/748e1c3a-f914-4adb-8ed7-925e84a0dc45">

In your personal workspace you can the upload the '1cHO inschrijvingen instelling.pbix'.

<img width="203" alt="Upload workspace" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/9be0125f-da98-41d0-a079-45bb6ad015e0">

If you want to publish the dashboard to the rest of your organisation a powerBI pro or premium license is needed.

# Usage
If you are using the desktop version just open 1cHO inschrijvingen instelling.pbix.

When using the online version go to your personal workspace and click on '1cHO inschrijvingen instelling' (type report).

<img width="462" alt="report workspace" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/911a465e-1171-41d5-b033-050fa0bbc985">

once in the report click on the edit button. 

<img width="745" alt="Edit" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/64b54ca2-d190-4655-b09e-865f663ec5e4">

From here you can edit the dashboard to your liking! PowerBI has a lot of functions and we will not discuss all of these here. Below you find a description of the functions that you can adjust in order to use the dashboard for your own organisation.

**Important!**
When using the desktop version make sure to adjust the FilePath parameter to the location where the input, header end supporting files are located. see below for an explanation on how to do this.

## Parameters
The dashboard has some build in parameters which let you adjust the default to fit your organisation's needs in data visualisation. Some of these parameters can remain on their defaults, others will need to be adjusted (for instance the filepath to the location of your input files).
In order to adjust the parameters click on the downward arrow below the 'Transform data' button. Then click on 'Edit parameters' 

<img width="523" alt="Edit parameters" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/0b7f99ea-31b3-4a0d-b54e-b14b5e860c11">

### FilePath
Change this parameter to the filepath where your input, header end supporting files are located (for instance: J:\NPuls\1cHO\\). Make sure to end the filepath with a "\\".

### Naam instellingsbestand
This parameter refers to the full name of the 1cHO inschrijvingen instellingsbestand. Usually this is in the form of "EV21XX24.036" or something similar. In the testinput provided in the package the name of the file is "EV21PL24.asc". However, for your own organisation there is no need to transform the originally provided file into .asc format. PowerBI is able to read in the file as is.

### Huidig jaar
This parameter refers to the current academic year of the 1cO inschrijvingen instellingsbestand. There are multiple measures which are linked to this parameter.

### Nationaliteit 1
In order to highlight certain nationalities in the visualisation there are 3 nationality parameters. There parameters can be adjusted to the nationality of your organisation's choosing. These take an integer value as input and are based on the Dec_nationaliteitscode.asc file, column "Code nationaliteit". The current value refers to Dutch.

### Nationaliteit 2
See nationaliteit 1. The current value refers to German.

### Nationaliteit 3
See nationaliteit 1. The current value refers to Belgian.

## Datatables
The data tab on the rightside shows a number of tables. These tables contain your data:

<img width="169" alt="Data tabellen" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/572c3349-b780-417d-9f06-2656409062f0">

The main table is the 'Inschrijvingen' table. This contains all the information from 1cHO file. The other tables are linked to this table in order to help with visualisation and calculations.

The datamodel button on the left will show you how the different tables are linked:

<img width="757" alt="Data model" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/b5342c0e-4636-4a00-9967-9461c2dbbac1">

## KPI
Currently the visualisations and tables in the dashboard are set to be able to show one of 4 KPI's. Which can be changed in the slicer in the top of the dashboard:

<img width="843" alt="KPI menu" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/03ea0136-e8c2-491e-a754-71d20a03e530">

These KPI's are:

  Aantal inschrijvingen: The total number of registrations
  
  Aantal instroom: The total inflow
  
  Aantal unieke inschrijvingen: The total number of unique registrations. This will only count one registration per student. Lets say one student has a bachelor and a master registration at the same time. In the total powerBI will count only one registration. If you would add program type to the visualisation powerBI would still count both the bachelor and master registration in each respective category, however the total would only still add up to one registration. This is because powerBI calculates the unique registration on each level of visualisation (once for all the bachelors, once for all the masters, and again for the total registrations).

  Aantal unieke instroom: The total number of unique inflow. The same rules apply as for the 'Aantal unieke inschrijvingen' KPI.

These KPI's are calculated as measures. Measures are extra transformations done on the data within the dashboard part of powerBI. In this particular dashboard you can find all the calculated measures in the 'KPI' folder under the 'Data' tab on the right:

<img width="383" alt="KPI measures" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/35d6906c-ba9c-4d97-b54a-9babada463b0">

Whenever you click on a measure you can see the calculation appear in the top center of the screen. Here you can adjust the code in order to adjust the measure.

<img width="1189" alt="Open measure" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/71d8d8e1-2faa-4766-8743-20c759917b51">

You can also create additional measures yourself by going to the home tab and clicking on 'New measure' in order to create the measure from scratch, or clicking on 'Quick measure' in order to get some suggestions and have the code already written for you.

<img width="819" alt="Measures quick and new" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/884b26a4-1dcd-4129-9968-1abd07827b94">

### Changing the settable KPI's
In order to have a different set of KPI's which the visualisations and tables can be set to you will need to adjust the 'KPI keuze' measure:

<img width="1188" alt="Variabele KPI" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/2d7c0059-13a6-46da-b522-4ea27c176b6f">

You can add additional KPI's in the form of: ("name you want shown in the slicer", NAMEOF('name of table'[measure or characteristic name]), integer which denotes order in the slicer). Additionally you can change the four KPI's already in the code by the same logic.

## Legend
Currently the visualisations and tables in the dashboard are set to be able to break down the data in 6 different characteristics. Once you choose one of these 6 characteristics powerBI will automatically change the legend to show this characteristic. You can change the legend by the slicer in the top of the dashboard:

<img width="843" alt="Legend slicer" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/ffdd41a7-1b95-49fe-8885-3b883366a327">

These characteristics are:

  Blank: Shows no breakdown and no additional legend items.

  Geslacht: Shows gender.

  Leeftijd: Shows age broken down in different age groups.

  Langstudeerder: Shows wether a student is a 'langstudeerder' or not. 'Langstudeerder' is defined as being in the nominal + 2 year of a study of the same program type. So for instance a 5th year bachelor student will count as 'langstudeerder', even if they changed bachelor program in between.

  Nationaliteitsgroep: Shows the nationalities cosen in the 3 nationality parameters + EEA other and Non-EEA other.

  Vooropleiding: Shows the highest completed previous education.

### Changing the settable Legend
In order to have a different set of characteristics for your legend which the visualisations and tables can be set to you will need to adjust the 'Legend' measure:

<img width="1188" alt="Legend measure aanpassen" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/5f054c5b-97b0-4be6-95a2-ed773e5c1566">

You can add additional characteristics in the form of: ("name you want shown in the slicer", NAMEOF('name of table'[measure or characteristic name]), integer which denotes order in the slicer). Additionally you can change the six characteristics already in the code by the same logic.

## Slicers
On the left of the dashboard there are seven slicers. With these slicers you can change which characteristics are shown:

<img width="139" alt="Slicers" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/8f51d091-8780-44c5-88e5-fd3ac2037c8b">

For instance, if you would change the 'Nationaliteits groep' slicer to 'Nederlandse' all the visuals will only show Dutch registrations. You can change multiple slicers at once and if the settings of one slicer would make for a certain characteristic in another slicer to not be there, then that slicer will not show that characteristic. For instance, if you would choose 'Nederlandse' again and there are no Dutch students under the age of 17, then the slicer 'Leeftijd' will not have the option '17 of jonger'.

You can change the content of the slicer by selecting the slicer in the dashboard, go to the visualisation tab and dragging another characteristic from the data tab to the field:

<img width="1253" alt="Aanpassen slicer" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/e3df0572-ef2d-4c3b-951a-1d6a22a32dca">

## Help, Table, and Graph view
On the left of the dashboard there are three clickable buttons:

<img width="380" alt="3 buttons" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/ded6e771-f5ec-44f0-99b4-80cc00dc2928">

The Help button, which shows an overlay with information regarding the dashboard:

<img width="383" alt="Help button" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/6018e7a6-35df-4419-b172-2b9c59ffd8bb">

The Table button, which will direct you to the table view (if you are not already in that view):

<img width="383" alt="Table button" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/66a16080-1bc1-40c9-aca4-a04e1079a75f">

And the Graph button, which will direct you to the graphics view (if you are not already in that view):

<img width="383" alt="Graph button" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/6d4c26b9-a0a6-4c2b-87ce-a96be70e1f29">

These powerBI buttons configured to follow certain bookmarks. To learn more about bookmarks visit: https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks?tabs=powerbi-desktop

## Json theme file
Included in the repository are multiple json files. These files contain a powerBI theme. In these files you can adjust the default background, used colours in graphs and tables, lettertype, effects of your visuals and lay-out.

In order to change the json used in your powerBI report go to the View tab, click on the downward arrow next to the them menu and select 'Browse for themes':

<img width="370" alt="theme upload" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/038eceee-ea5d-416b-9ff3-487b855bfd35">

Now you can select your json file and use this as your theme.

### Background
In order to change the background used in the json file you will first need to create a background image. For the uploaded json files powerpoint was used to create the background. After an image has been created this will need to be converted to base64 code. A useful website for this is https://www.base64-image.de/.

After the conversion you can fill the code after "url" in the background image element in the json file:

<img width="1026" alt="Background base64" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/b39c7326-a6b2-4597-99c8-208daa3f1bef">

### DataColors
In order to change the colours that are used in all your graphs you will need to change the "DataColors" element in the json:

<img width="205" alt="DataColors" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/9bb66a09-f14c-4e9c-9253-3b4993806214">

These are in HEX notation.

### TextClasses
You can also change the default font, size, and color of your text in all of your objectsin powerBI. This is done in the "textClasses" element in the json file:

<img width="316" alt="Textclasses" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/9bcd0cb7-967f-4883-8130-92c561ef9cfd">
