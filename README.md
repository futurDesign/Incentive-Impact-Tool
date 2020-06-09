# Incentive-Impact-Tool
This is a tool that allows users to visualize the impacts of electric vehicle incentive attributes.

## Organization:

### ui.R
This file contains the front-end ui code. It makes use of shinydashboard, shinyBS, and shinyjs.

## server.R
This file performs the reactive calculations to supply outputs for the ui.

## util.R
This file contains helper functions for calculations and plots referenced by server.R and report.Rmd.

## global.R
This file contains code to load in the databases that are used by the app. It also contains some code that defines a few conversion constants using the units package.

## Incentive Impact Tool.Rproj
The R project file, useful to open when editing any R file.

## www
At the top level, there are two logos used by the app

### Data Tables
* State Info and Vehicles: these folders contain data tables in csv format. These can be edited when adding new vehicles, mixes, electricity generation profiles, etc.
* process_data_for_web_use.R: this file is used to convert the csv files to the data.RData file that is used by the app. This saves some server load on the back end.
* data.RData: the aforementioned data file that is generated by process_data_for_web_use.R
* NHTS_state_autotrip_info.R: Obtaining vehicle level VMT from the NHTS by state is a little tricky. This script should be used with NHTS/trippub.csv to calculate a list of mean vehicle VMT and number of trips per day.
