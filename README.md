# WEATHER Data Management and Monitoring

This project reads, cleans and monitors the data that is being collected in the WEATHER project from MOZAMBIQUE.

## Info

* **Network folder**: `airpollution/MOZAMBIQUE/FC_mozambique-weather-data`
* **Maintainer**: Fabian Coloma
* **Collaborators**: Ariadna Curto, Jovito Nunes

All paths below are relative to the root of the project folder. As an additional way to work with, you can clone or acces by `https://github.com/isg-airpollution/FC_mozambique-weather-data.git` or [entry on repository](https://github.com/isg-airpollution/FC_mozambique-weather-data)

### Structure

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


