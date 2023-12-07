# CME538-Big-Project - Movie Revenue Estimator

## Project Overview
The Movie Revenue Estimator is a predictive model that estimates movie revenues. It leverages data-driven insights from various sources such as TMDB, Box Office Mojo, Rotten Tomatoes, and YouTube. Our model analyzes factors like genres, keywords, cast details, and more to make accurate predictions.

## Repository Structure
This repository contains the following components:
- **Jupyter Notebooks**: Five notebooks each with a specific purpose in the data extraction and analysis process.
- **Data Folders**: Two folders - 'Yearly' and 'AdditionalData' for organized data storage.

## Jupyter Notebooks Overview
### TMDB Yearly Data Extractor.ipynb
- **Purpose**: Extracting data from the TMDB website
- **Import Libraries**: Begins with importing necessary libraries for concurrent processing and web requests.
- **Define Functions**: Includes functions to fetch movie details, keywords, and cast from TMDB.
- **Concurrent Data Fetching**: Implements concurrent fetching for efficiency.
- **Setup and Loop**: Sets up API key, date ranges, and executes a loop for data extraction.
- **Save Data**: Outputs the data into a CSV file.

### Box_office_mojo_scrape.ipynb
- **Purpose**: Scrapes movie revenue data from Box Office Mojo.
- **Install BeautifulSoup**: Installs and imports BeautifulSoup for web scraping.
- **Import Libraries**: Loads necessary Python libraries for HTTP requests and data handling.
- **URL Setup**: Sets up the URL for Box Office Mojo scraping.
- **Scrape Process**: Implements scraping logic using BeautifulSoup.
- **Data Processing**: Processes and structures the scraped data.
- **Save/Export Data**: Outputs the data into a CSV file.

### Web_Scrape_Rotten_Tomatoes.ipynb
- **Purpose**: Scrapes movie score data from Rotten Tomatoes.
- **Read Data**: Begins by reading a CSV file containing movie data.
- **URL Setup**: Sets up search URLs for Rotten Tomatoes.
- **Scrape Function**: Defines functions for scraping Rotten Tomato scores.
- **Scrape Scores**: Scrapes scores for each movie.
- **DataFrame Creation**: Organizes the data into a DataFrame.
- **Data Cleaning and Saving**: Cleans and saves the data to CSV.

### Youtube API.ipynb
- **Purpose**: Scrapes movie data from Youtube
- **Library Setup**: Installs Google API client and imports libraries.
- **Read Data and API Setup**: Reads a CSV for movie titles and sets up YouTube API.
- **Define Retrieval Functions**: Functions for retrieving YouTube video engagement and comments.
- **Video Search and Data Extraction**: Searches for relevant videos and extracts data.
- **Fetch Comments**: Retrieves top comments for each video.
- **Data Storage and Output**: Stores data in lists and prints details.
- **DataFrame and CSV Export**: Creates DataFrame and exports to CSV.

### Detailed Instructions for Each Notebook
### TMDB Yearly Data Extractor.ipynb
This notebook contains code for extracting data from the TMDB website. To use it effectively, follow these steps:

**Variable Adjustment:** Modify the "year" variable within the code to specify the year for which you want to extract data.

**Output:** The result of running this code is a CSV file named "year.csv" with the following columns: 

1. **adult**: Indicates if the movie content is intended for adults.

2. **backdrop_path**: URL or path to the backdrop image of the movie.

3. **belongs_to_collection**: Information about the collection to which the movie belongs.

4. **budget**: The budget allocated for the movie's production.

5. **genres**: Genres associated with the movie.

6. **homepage**: URL to the movie's official website.

7. **id**: Unique identifier for the movie.

8. **imdb_id**: IMDb identifier for the movie.

9. **original_language**: The original language in which the movie was released.

10. **original_title**: The original title of the movie.

11. **overview**: A brief overview or summary of the movie's plot.

12. **popularity**: A popularity score or ranking for the movie.

13. **poster_path**: URL or path to the movie's poster image.

14. **production_companies**: Information about production companies involved in the movie.

15. **production_countries**: Countries associated with the movie's production.

16. **release_date**: The date on which the movie was released.

17. **revenue**: The movie's revenue or earnings.

18. **runtime**: The duration of the movie in minutes.

19. **spoken_languages**: Languages spoken in the movie.

20. **status**: The status of the movie (e.g., released, in production).

21. **tagline**: A tagline or slogan associated with the movie.

22. **title**: The title of the movie.

23. **video**: Indicates if the movie has a video available.

24. **vote_average**: Average user rating or vote score.

25. **vote_count**: The total number of votes or ratings received.

26. **keywords**: Keywords or tags associated with the movie.

27. **cast**: Information about the cast members in the movie.


### Box_office_mojo_scrape.ipynb
This notebook contains code for extracting data from the MOJO website. To use it effectively, follow these steps:

**Variable Adjustment:** Modify the dates list within the code to specify the dates for which you want to extract data.

**Output:** The result of running this code is a CSV file named "gross_earning_domestic_2013-2023.csv" with the following columns: 

1. **movie**: The title of the movie

2. **daily earnings**: Daily earnings generated from the movie

3. **threatres**: The number of theaters where the movie was screened

4. **earnings_per_theatre**: The average earnings per theater for the movie. 

### Web_Scrape_Rotten_Tomatoes.ipynb
This notebook contains code for extracting data from the Rotten Tomato website. To use it effectively, follow these steps:

**Variable Adjustment:** Modify the file list within the code to specify the movies you want the scores for.

**Output:** The result of running this code is a CSV file named "gross_earning_domestic_2013-2023.csv" with the following columns: 

1. **movie**: The title of the movie

2. **Specific Rotten Tomato score**: Rotten Tomato score

### Youtube API.ipynb
This notebook contains code for extracting data from the Youtube website. To use it effectively, follow these steps:

**Variable Adjustment:** Modify the '.csv' file within the code to the movies column to get the youtube data from it.

**Output:** The result of running this code is a CSV file named "movies_with_engagement_and_comments" with the following columns: 

1. **MovieTitle**: The title of the Movie Title

2. **Youtube Video Title**: The movie Title

3. **Youtube Video ID**: The youtube video id

4. **Views**: The view count of the youtube video

5. **Likes**: The likes count of the youtube video

6. **Comments**: The comment count of the youtube video

7. **Top 10 Comments**: The top 10 comment is the video separted by '|,'

**Notes:** When using the Youtube API, please refer to the guide below for additional resources for help.
## Usage
After running each notebook, save the outputs in their respective folders. Ensure correct placement of files for seamless operation of the EDA pipeline.

## Dependencies
- Python 3.8+
- Pandas, NumPy, Matplotlib, Seaborn
- API Keys for TMDB, YouTube
- Additional libraries: (list any other specific libraries or frameworks used)

## Installation
Provide instructions for setting up the environment and installing necessary dependencies.

## Running the Model
Explain how users can run the model after setting up the environment and processing the data.

## License
(Include license information here.)

## Contact Information
For inquiries or contributions, please contact Blueboy at ansonlam77@gmail.com

## Additional Resources
- [TMDB API Documentation](link)
- [YouTube API Guide](link)
- (Any other relevant links or resources)

---

This format ensures that your README is informative and user-friendly, guiding users through the process of utilizing your project effectively. Don't forget to include any additional information or instructions specific to your project's requirements.
