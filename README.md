# Analysing Parking Behaviour in Amsterdam Using Agent Based Modelling (Internship Project 2019 - CWI, Amsterdam)
This repo contains all information regarding my data science master thesis about the evaluation of the agent-based parking model SimPark as a parking policy tool. This evaluation will be done with a case where on-street parking places were moved off-street in the Frans Halsbuurt. This case will be split up in three parts.

## Case
Parking situations Frans Halsbuurt:
1. May 2018 - 567 parking places on-street
2. Oct 2018 - 567 parking places on-street and 600 parking places off-street
3. Feb 2019 - 81 parking places on-street and 600 parking places off-street

## Repo structure
### Data
All public data that is needed for the scripts and the model is stored in this folder.

### Documents
In this folder all documents created for/on meetings etc. are stored.

### Papers
All papers used for this research are stored in this folder.

### Scripts
These three parking situations will be simulated with the agent-based parking model SimPark. All agents (drivers) will be modeled separately and will drive there own trips. These trips will be obtained through OViN data. This data contains all trips a person makes during one day of the year.  To generate agents for the simulation trips are generated in scripts/schedules_generator.py and outputs an xml file for SimPark. This xml file is stored in data/generated/xml.

To generate the parking facilities and parking regulations parking facility and regulation data from the City of Amsterdam is used. This data is processed in scripts/parking_generator.py and outputs an xml file for SimPark. This xml file is stored in data/generated/xml.

The road network from the Frans Halsbuurt for SimPark is obtained via OpenStreetMap. This xml file is stored in data/generated/xml.

The vehicles used in SimPark are stored in data/generated/xml.

All files in data/generated/xml are input files for SimPark.




