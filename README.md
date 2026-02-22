# IG/G lab on data platforms

# Getting started
    - 1. $ git clone "the-url-to-this-repo"
    - 2. Navigate to the new local repo and activate your virtual environment
    - 3. $ uv sync
    - 4. Navigate to transformations.ipynb, change kernel and run to generate results

# Theory questions

# 1. Ingest -> Storage -> Transform -> Access
    - Describes the journey of data, from raw source to presentable information
    - Ingestion: gathering of raw data and bringing it into the system, like downloading the untouched CSV-file in this lab
    - Storage: where the data actually exist, in this case locally and through git version control / github
    - Transform: 'cleaning' raw data through date standardization, removing blank spaces and type conversion (check out 'Data     Cleaning' inside this repos .ipynb)
    - Access: final presentation of data through analysis, dashboards et cetera (like we have done through analyzing the average of prices)

# 2. Summary of pandas, psycopg3 and pydantic
    - pandas: library in python that provide functionality that lets you clean and analyze data in memory as well as new data structures like 'Series' (single column) and 'Dataframes' (table - like)
    - psycopg3: library in python that enables communication between local machinery and postgreSQL. So while data may be cleaned locally using pandas, storage is provided by postgreSQL, and the gap between the two is bridged using psycopg3
    - pydantic: library in python that help validate records through schema structure enforcements, type enforcement and other constraints. It is useful when you want to ensure data correctness when working with API:s

# 3. Extract -> Transform -> Load
    - Extract: gathering raw data from, for example, CSV-files or API:s
    - Transform: cleaning the raw data through, for example, formatting and duplicate-removals, in order to make it consistent, accurate and, thusly, ready for analysis
    - Load: storing the cleaned data in its destination, like files or databases, and making it accessible