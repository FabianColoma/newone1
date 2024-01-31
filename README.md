# WEATHER Data Management and Monitoring

This project reads, cleans and monitors the data that is being collected in the WEATHER project from MOZAMBIQUE.

## Info

* **Network folder**: `airpollution/MOZAMBIQUE/FC_mozambique-weather-data`
* **Maintainer**: Fabian Coloma
* **Collaborators**: Ariadna Curto, Jovito Nunes

All paths below are relative to the root of the project folder. 

As an additional way to work with, you can clone or access by `https://github.com/isg-airpollution/FC_mozambique-weather-data.git`

## Data 

> The data is loading by two sources. 

*It's important to take note that the second step is a back-up to the first step. That implies that if the first one is not working or no one is doing the process, the web will not have new information.*

1 - The first load is performed manually. The data must be downloaded on a bi-weekly basis to avoid data being over writter, the data that is stored on the data logger is kept in the data logger fo 21 day, after this the data is overwritten. 

- Using WeatherLink software, data can be downloaded and included in yoyt WeatherLink data files stored in the PC.
- download the data by connecting your laptop to the data logger via USB cable.

2 - The second source involves requesting the [API](https://www.weatherlink.com/). 


**For more information go to the description on [Readme_weatherlink_v2](../main/documents/)**

## Structure

* The raw data and processed data is in folder `data/`.

* Documentation and data dictionary are in folder `documents/`

* `Output/` there will be recollected all the outcomes that we need to made analysis 

* The [`R/`](R) folder contains the functions needed to read and process the raw data. not just R code, that development include python.

* Extended analisis and markdown files will be posted on `reports/`

* The whole processing pipeline is orchestrated by [`run.R`](run.R). In this case we dont use this file, because the development involve python.. for this reason the below bloc will explain the process.


## Processing pipeline

1. The first part the raw data must be manually uploaded to the `data/raw-data/` folder.

>  To ensure that the API key stays within the system, please keep the Python code on the cluster and do not share it.

2. `R/conection_api.py` this file contain the steps to make the first request to the API, and get the station ID that we will need to made the other request.

3. `R/historical_request_1_day.py` This file made a historical request by 1 day, this is the base to made the sequential download.

4. `R/historical_multi_request.py` This file have the generalization and the lastest version of the download process. For this reason that one will be used to continue the request. You can find a extended explanation on [Readme_weatherlink_v2](../main/documents/)

5. `R/weather-data.Rmd` The first load and treatment of the data from data logger.

**To begin modifying or executing the code for the first time, it's advisable to copy it to a `scratch/` folder or clone a repository from Github.**

## Analysis

Comparing the two sources, the unique difference is the units.

