# Palmeiras Analytics BR

This is my captstone project to my MBA in Data Science and Analytics from USP/ESALQ (Brazil), under the guidance of professor Patricia Belfiore Fávero. It aims to analyze the data from a Brazilian football team Palmeiras (SEP) along the Brazilian Championship during 2020 to 2023.

## Structure
```bash
palmeiras_analytics_br/
├── json_renamed/                           # JSON files scrapped from Sofascore with all Palmeiras matches. There are 5 different types of them.
│   └── j_DDMMYYYY_ID_event.json
│   └── j_DDMMYYYY_ID_incidents.json
│   └── j_DDMMYYYY_ID_lineups.json
│   └── j_DDMMYYYY_ID_shotmap.json
│   └── j_DDMMYYYY_ID_stats.json
├── notebooks/                              # Notebooks
│   └── data_wrangling/                     # Notebooks with JSON data wrangling 
│       └── wrangling_events.ipynb          # Data wrangling JSON with event data and generating events.csv as output
│       └── wrangling_incidents.ipynb       # Data wrangling JSON with incident data and generating incidents.csv as output
│       └── wrangling_lineups.ipynb         # Data wrangling JSON with lineups data and generating lineups.csv as output
│       └── wrangling_shotmap.ipynb         # Data wrangling JSON with shotmap data and generating shotmap.csv as output
│       └── wrangling_stats.ipynb           # Data wrangling JSON with stats data and generating stats.csv as output
├── .gitignore                              # Files to be ignored for Git
├── README.md                               # Documentation about this project
├── pyproject.toml                          # Poetry project setup file
└── poetry.lock                             # Poetry dependency lock file

```

## Dependencies

This project uses Python and these packages:

- pandas
- numpy
- matplotlib
- scikit-learn

To install all the dependencies, use use [Poetry](https://python-poetry.org/):

```bash
poetry install
