IMDb Movie Details Scraper
This Python script uses Selenium to scrape movie details from IMDb's "Top 250" movie chart. The script navigates to the IMDb website, extracts information for each movie, and organizes the data into a Pandas dataframe. Additionally, it allows users to filter movies based on their preferences.

Script Overview
Importing Libraries: The script starts by importing necessary libraries, including Selenium for web scraping and Pandas for data manipulation.

Setting Up WebDriver: The Chrome WebDriver is initialized using the webdriver module from Selenium, and the IMDb website's URL is opened.

Data Extraction: Movie details such as title, runtime, rating, age restriction, writers, directors, genre, and trivia are extracted from each movie card on the IMDb "Top 250" chart.

Organizing Data: The extracted information is stored in a dictionary called movies, which is then converted into a Pandas dataframe. The dataframe is saved as a CSV file.

User Input and Filtering: Users are prompted to input their movie preferences, including genre, minimum rating, maximum runtime, and age restriction. The script then filters the movies based on these preferences, calculating the total runtime in minutes.

Random Selection: If no movie matches the user's preferences, a random movie is selected from the original dataset.

Displaying Results: The final filtered dataframe is displayed, showcasing movies that match the user's criteria.
