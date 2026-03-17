## Movie Scraper Project (Top 50 Films)
I built this script to scrape movie data from a wiki archive. It grabs the top 50 highest-ranked films and saves them into a CSV and a local SQLite database.

How to set it up
You'll need a few Python libraries to run this. You can install them all at once:
pip install requests pandas beautifulsoup4

Running the script
Once you have the libraries, just run the .py file:

Bash
python3 webscraping_movie.py
What you get
When the script finishes, it creates two files in your folder:

top_50_films.csv - A clean spreadsheet of the movies.

Movies.db - An SQLite database file with the same data.

The Code Logic
Scraping: Uses BeautifulSoup to find the tbody and tr tags in the HTML.

Data Handling: Uses Pandas to structure the "Average Rank", "Film", and "Year".

Storage: Uses sqlite3 to connect to a local database and swap out the old data for the new scrape.
