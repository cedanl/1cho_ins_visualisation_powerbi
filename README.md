# 1cho_ins_visualisation_powerbi
Each Higher Education institution receives the 1cHO_inschrijvingen_instellings_bestand once a year. This file contains data regarding the registrations of all their current students. The files in this package contain a fully working powerBI dashboard ready to run on the 1cHO_inschrijvingen_instellings_bestand and all accompanying supportfiles without the need for any further data transformations on these files.

# Installation
A prerequisite for running this package is the installation of powerBI. A free to use download can be found here: https://powerbi.microsoft.com/en-us/downloads/. The desktop version of powerBI is free to use. However, if you want to publish the dashboard to the rest of your organisation a powerBI pro or premium license is needed.

"Download" the raw file 1cHO inschrijvingen instelling.pbix, NPuls Theme aanpas.json, the header_files, the supporting_files, and the input.

# Usage
Open 1cHO inschrijvingen instelling.pbix The dashboard has some build in parameters which let you adjust the default to fit your organisation's needs in data visualisation. Some of these parameters can remain on their defaults, others will need to be adjusted (for instance the filepath to the location of your input files).

## Parameters

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
