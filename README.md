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

- The initial update is performed manually every 21 days or less.  The description is on [Readme_weatherlink_v2](../main/documents/) inside of the 1rt BLOCK.

- The second source involves requesting the [API](https://www.weatherlink.com/). This part is explained on [Readme_weatherlink_v2](../main/documents/) inside of the 2on BLOCK.

*It's important to take note that the second step is a back-up to the first step. That implies that if the first one is not working or no one is doing the process, the web will not have new information.*


* The raw data is in folder `raw-data/`.

* The [`R/`](R) folder contains the functions needed to read and process the raw data.

* The whole processing pipeline is orchestrated by [`run.R`](run.R).

* The processed data is stored in the `processed-data/` folder.

## Data

The raw data must be manually uploaded to the `raw-data/` folder following the structure specified in the SOPs.

## Data

> The data is confidential and therefore not version controlled but can be accessed upon request.

The `data/` folder contains the following raw data files:

* `dataset_1.csv`: Brief description

* `dataset_2.csv`: Brief description

## Analysis

The analysis pipeline is orchestrated by [run.R](run.R).

## Output

Specify the output files of the project.

## How to reproduce


``` bash
.
├── Manhica
│   ├── Season 1
│   │   ├── 999-99999
│   │   │   ├── EXACT
│   │   │   ├── FOTOS
│   │   │   ├── HAPEX
│   │   │   └── UPAS
│   ├── Season 2
│   │   ├── 999-99999
│   │   │   ├── EXACT
│   │   │   ├── FOTOS
│   │   │   ├── HAPEX
│   │   │   └── UPAS
└── Xinavane
    ├── Season 1
│   │   ├── 999-99999
│   │   │   ├── EXACT
│   │   │   ├── FOTOS
│   │   │   ├── HAPEX
│   │   │   └── UPAS
│   ├── Season 2
│   │   ├── 999-99999
│   │   │   ├── EXACT
│   │   │   ├── FOTOS
│   │   │   ├── HAPEX
│   │   │   └── UPAS

```


