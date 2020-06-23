
The dataset used in the tableau dashboard: Movebank_yellowLoonAnnotated_v2.csv

Metadata table used by Tableau: input: YellowLoonStudyNotes.xlsx,  Tableau generated: Clipboard_20200503T185058.txt


The Env-DATA Track Annotation Service

The Env-DATA Track Annotation Service allows Movebank users to add environmental information to animal tracking data 
and related time-location records. This information includes hundreds of variables that are part of global environmental 
datasets provided by the European Centre for Medium-Range Weather Forecasts (ECMWF), the European Space Agency (ESA), 
the National Aeronautics and Space Administration (NASA), the US National Oceanic and Atmospheric Administration (NOAA), 
and others. You can browse information about available datasets here. The Env-DATA Track Annotation Service allows you to 
select what data to annotate, browse and select environmental variables, choose data interpolation methods, and submit an 
annotation request.

https://www.movebank.org/cms/movebank-content/env-data-track-annotation

The Env-Data service requires users to request environmental variables manually. In this use case, requesting all of the
environmental variables at once led to service failures. Therefore, each data set was requested individually and then 
processed + combined in the file Movebank_yellowLoonAnnotated_v2.csv. Wind speed, wind direction, land use, and air 
temperature are used as linked environmental variables for the species migration dashboard. The raw data are provided 
in respective folders with metadata readme files for this exploratory case.  In future practice, a REST API would improve
the capability to reproduce linked environmental data used in a dashboard. 

