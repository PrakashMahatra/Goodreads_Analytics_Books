

# Goodreads Books Data Analytics

## Overview
This project involves analyzing data obtained from Goodreads, a popular website for book lovers, to gain insights into the best books of the 21st century. The data was scraped from the [Best Books of the 21st Century](https://www.goodreads.com/list/show/7.Best_Books_of_the_21st_Century) list on Goodreads using the Beautiful Soup and Requests libraries in Python. After obtaining the data, cleaning and exploratory data analysis (EDA) were performed using Pandas, Plotly, Seaborn, and Matplotlib.

## Table of Contents
- [Project Description](#goodreads-books-data-analytics)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Data Scraping](#data-scraping)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Conclusion](#conclusion)
- [Future Work](#future-work)

## Project Structure
- `notebooks/`: Contains Jupyter notebooks used for data scraping, cleaning, and EDA.
- `data/`: Contains the dataset obtained from the Goodreads website and any intermediate datasets created during the project.
- `Plots.doc`: **QUICK VIEW ON PLOTS AND GRAPHS**.
- `README.md`: The README file providing an overview of the project.
- `Requirements.txt`: All libraries and tools needed for this project. 

## Technologies Used
- Python
- Beautiful Soup
- Requests
- Pandas
- Plotly
- Seaborn
- Matplotlib
- Numpy

## Data Scraping
Data was scraped from the [Best Books of the 21st Century](https://www.goodreads.com/list/show/7.Best_Books_of_the_21st_Century) list on Goodreads using the Beautiful Soup and Requests libraries in Python. The scraped data includes information such as book titles, authors, ratings, and reviews.

## Data Cleaning
Upon scraping the data, cleaning was performed to handle missing values, remove duplicates, and ensure consistency in the data. This step involved preprocessing the data to make it suitable for analysis.
#### What i did in this notebook-->
** Dirty Data**
- Remove null values from the datset
- **first_published column**: remove first published text and change its format to datetime.
- **ratings column**: remove ratings text from infront of the number.
- **Change** all columns to their **respective formats.**
- Change syntax of column names
- Remove text from the column **author_followers and no_of_reviews**
- Remove text from **Total_pages** column.
- Remove (,) and (1%) part from **one_star,two_star**,etc columns.
- change column  **avg_ratings to toTal_ratings**
- Drop column **Rating**
- Some values in column **Author_followers**has inconsistent values like 1boo576,1boo890 etc 
- Two columns **Author_followers and Reviews ** has invisible special charaters The values are strings containing numeric characters along with non-printable characters like \xa0, which is the Unicode representation of a non-breaking space.**
- Remove books with page less than 20.
- Multiplying author folowers with 1000 so to convert 'k' into numeric form.

## Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) was conducted using Pandas, Plotly, Seaborn, and Matplotlib to gain insights into the dataset. Visualizations such as histograms, bar plots, scatter plots, and heatmaps were created to analyze various aspects of the data, including book ratings, authors, genres, and publication years.
#### Few questions i tackled:  -->
- Which authors have the highest average ratings and significant number of ratings?
- How does the number of pages correlate with the book's average rating?
- How are the 5-star ratings distributed among books with different average ratings?
- What is the average number of ratings per book by genre?
- Is there a relationship between the total number of reviews and the average rating?
- What are the characteristics of the top 1% of books based on 5-star ratings?
- What is the trend of book publications over time by the top authors?
## Conclusion
The analysis provided valuable insights into the best books of the 21st century, including trends in book ratings, popular authors, genres, and publication years.



---

