Overview

This project focuses on web scraping, cleaning, and transforming tabular data from a web page into a structured format using Python. The primary objective is to extract a table containing population and demographic information about Canadian provinces, clean the data, and convert it into a structured format for further analysis.

Features

Web Scraping: Extracts table data, including header and rows, from a web page using BeautifulSoup.

Data Cleaning: Handles formatting issues such as commas and percentage signs in numeric data.

Data Transformation: Converts cleaned data into a structured Pandas DataFrame for analysis.

Technologies Used

Python: The primary programming language for this project.

BeautifulSoup: For parsing HTML and extracting data from the web page.

Pandas: For data manipulation and cleaning.

Installation

Clone this repository:

git clone https://github.com/yourusername/your-repo-name.git

Navigate to the project directory:

cd your-repo-name

Install the required Python packages:

pip install -r requirements.txt

Usage

Run the script to scrape and clean data:

python main.py

View the cleaned data in the console or save it to a file for further analysis.

Workflow

Scrape Data:

Extracts the table, headers, and rows using BeautifulSoup.

Handles nested elements such as anchor tags for province names.

Clean Data:

Removes unwanted characters (e.g., commas, percentage signs) from numeric columns.

Converts columns to appropriate data types.

Transform Data:

Converts the cleaned rows and headers into a Pandas DataFrame.

Validates the final DataFrame structure.

Example Output

         Province   2024 Pop.   2022 Pop.   2016 Pop.   2011 Pop.  Change
0        Ontario  15996989  15262660  13448494  12851821    2.19
1         Quebec   9030684   8751352   8164361   7903000    1.27
...

Known Issues

Ensure the table structure on the target webpage remains consistent; any changes might require updates to the scraping logic.

Columns with mixed data types (e.g., numeric and text) may need additional cleaning steps.
