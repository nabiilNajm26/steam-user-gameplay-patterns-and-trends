
# Analysis of Steam User Gameplay Trends and Patterns

## Project Background
In the digital age, game distribution platforms like Steam have become a rich source of data on user behavior and preferences. With over 100 million user reviews, this data provides valuable insights into trends and patterns in user gameplay that can be leveraged by game developers, marketers, and researchers. This project aims to analyze the trends and patterns of Steam users' gameplay, focusing on various aspects such as playtime, game popularity, and gameplay behavior based on time and region.

## Problem Statement
This project aims to answer several key questions:
- How do user gameplay patterns change over time (e.g., weekends vs. weekdays)?
- What games are the most popular in different regions?
- How much time do users spend playing certain games?

By answering these questions, this project will provide insights that can be used to optimize marketing strategies, game development, and user experience enhancement.

## Dataset
- **Source:** Steam user reviews dataset
- **Size:** 17 GB (compressed), 43.19 GB (extracted)
- **Columns:** 24 columns including `recommendationid`, `appid`, `game`, `author_steamid`, `author_playtime_forever`, `author_playtime_last_two_weeks`, `timestamp_created`, etc.

## Tools and Technologies
- **Docker**: For container management
- **Python**: Main programming language
- **Polars**: For data processing and transformation
- **Apache Airflow**: For managing the batch processing pipeline
- **PostgreSQL/MySQL**: For storing processed and analyzed data
- **Grafana/Metabase**: For visualizing the analysis results in interactive dashboards

## Installation and Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/steam-user-behavior-analysis.git
   cd steam-user-behavior-analysis
   ```

2. **Setup Docker**
   - Install Docker from [here](https://docs.docker.com/get-docker/)
   - Build and run the Docker container
     ```bash
     docker-compose up --build
     ```

3. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Data Processing Pipeline
1. **Data Extraction**
   - Extracting Steam review data from the provided dataset.
   - Using Polars to load the data.

2. **Data Cleaning**
   - Cleaning data to remove missing or invalid values.
   - Using Polars for data cleaning operations.

3. **Data Transformation**
   - Calculating user playtime statistics such as total playtime, playtime in the last two weeks, etc.
   - Grouping data by time (e.g., weekends vs. weekdays) and region.

4. **Data Storage**
   - Storing analysis results in PostgreSQL or MySQL databases.

5. **Visualization**
   - Creating dashboards using Grafana or Metabase to display the analysis results.

## Project Structure
```
steam-user-behavior-analysis/
│
├── data/                   # Folder to store datasets
│
├── dags/                   # Folder to store Airflow DAGs
│   ├── data_extraction.py
│   ├── data_cleaning.py
│   ├── data_transformation.py
│   └── data_storage.py
│
├── notebooks/              # Jupyter notebooks for data exploration and initial analysis
│   └── EDA.ipynb
│
├── scripts/                # Folder to store Python scripts
│   ├── extract_data.py
│   ├── clean_data.py
│   ├── transform_data.py
│   └── store_data.py
│
├── requirements.txt        # List of Python dependencies
│
├── docker-compose.yml      # Docker Compose file
│
└── README.md               # This document
```

## Expected Output
1. **Analysis Report**
   - User playtime statistics based on time and region.
   - Charts and tables showing gameplay trends and game popularity.

2. **Visualization Dashboard**
   - Interactive dashboard displaying analysis results in charts and diagrams.
   - Filter features to view data by time, region, and specific games.

3. **Project Documentation**
   - Comprehensive documentation explaining each step in the project, including environment setup, data processing, and result interpretation.

4. **Presentation**
   - Presentation slides summarizing the project, analysis results, and recommendations for the audience.

## Conclusion & Recommendation
1. **Conclusion**
   - This platform can effectively process and present Steam user gameplay data.
   - Provides valuable insights for game development and marketing strategies.

2. **Recommendation**
   - Further integration with game sales data for deeper analysis.
   - Using machine learning for predicting future gameplay trends and patterns.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements
Special thanks to everyone who contributed to the completion of this project, including mentors and colleagues in Data Engineering Batch 5.
