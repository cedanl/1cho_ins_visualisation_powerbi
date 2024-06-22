# 1cho_ins_visualisation_powerbi
Each Higher Education institution receives the 1cHO_inschrijvingen_instellings_bestand once a year. This file contains data regarding the registrations of all their current students. The files in this package contain a fully working powerBI dashboard ready to run on the 1cHO_inschrijvingen_instellings_bestand and all accompanying supportfiles without the need for any further data transformations on these files.

# Installation
A prerequisite for running this package is being able to run powerBI, either the online version or the desktop version. The recommendation is to use the desktop version, however for the purposes of the demo the online version should suffice.

For both options you will need to download or pull the raw file 1cHO inschrijvingen instelling.pbix, NPuls Theme aanpas.json, the header_files, the supporting_files, and the input.

### How to install the desktop version:
You will need to download and install powerBI. A free to use download can be found here: https://powerbi.microsoft.com/en-us/downloads/. The desktop version of powerBI is free to use. However, if you want to publish the dashboard to the rest of your organisation a powerBI pro or premium license is needed.

### How to install the online version:
The prerequisite for this option is that your organisation as some sort of microsoft licence. If your organisation uses microsoft teams, this should be in order. Go to https://app.powerbi.com and log in with your organisation's email account. Once you have logged in you can open your personal workspace (located in the left menu).
<img width="55" alt="My workspace" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/748e1c3a-f914-4adb-8ed7-925e84a0dc45">
In your personal workspace you can the upload the '1cHO inschrijvingen instelling.pbix'. <img width="203" alt="Upload workspace" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/9be0125f-da98-41d0-a079-45bb6ad015e0"> If you want to publish the dashboard to the rest of your organisation a powerBI pro or premium license is needed.

# Usage
If you are using the desktop version just open 1cHO inschrijvingen instelling.pbix.

When using the online version go to your personal workspace and click on '1cHO inschrijvingen instelling' (type report).<img width="462" alt="report workspace" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/911a465e-1171-41d5-b033-050fa0bbc985"> once in the report click on the edit button. <img width="745" alt="Edit" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/64b54ca2-d190-4655-b09e-865f663ec5e4">

From here you can edit the dashboard to your liking! PowerBihas a lot of functions and we will not discuss all of these here. Below you find a description of the functions that you can adjust in order to use the dashboard for your own organisation.

## Parameters
The dashboard has some build in parameters which let you adjust the default to fit your organisation's needs in data visualisation. Some of these parameters can remain on their defaults, others will need to be adjusted (for instance the filepath to the location of your input files).
In order to adjust the parameters click on the downward arrow below the 'Transform data' button. Then click on 'Edit parameters' <img width="523" alt="Edit parameters" src="https://github.com/ed2c/1cho_ins_visualisation_powerbi/assets/97895708/0b7f99ea-31b3-4a0d-b54e-b14b5e860c11">

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

## KPI
Currently the visualisations and tables in the dashboard are set to be able to show one of 4 KPI's. These KPI's are:
  Aantal inschrijvingen: The total number of registrations
  Aantal instroom: The total inflow
  Aantal unieke inschrijvingen: The total number of unique registrations. This will only count one registration per student. Lets say one student has a bachelor and a master registration at the same time. In the total powerBI will count only one registration. If you would add program type to the visualisation powerBi would still count both the bachelor and master registration in each respective category, howver the total would only still add up to one registration. this is because powerBI calculates the unique registration on each level of visualisation (once for all the bachelors, once for all the masters, and again for the total registrations).
