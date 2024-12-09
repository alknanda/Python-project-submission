IMDB Movie Scraper

IMDB Movie Scraper is a web application built with Flask that allows users to search for movies by genre. The application scrapes movie data from IMDB and displays the top 5 movies for the specified genre, including the title, year, rating, and metascore.
Features

    Search by Genre: Users can search for movies by entering a genre (e.g., action, comedy, drama).
    Top 5 Movies: The application displays the top 5 movies for the specified genre.
    Dynamic Title: The title on the results page reflects the genre searched by the user (e.g., "Top 5 Action Movies”).
    Error Handling: The application handles invalid genre inputs and displays user-friendly error messages.
    User-Friendly Interface: Built with Bootstrap, the application provides a clean and responsive user interface.

Technologies Used
Backend

    Flask: A lightweight WSGI web application framework in Python used to build the web server.
    BeautifulSoup: A Python library used for web scraping to extract movie data from IMDB.
    Requests: A simple, yet powerful HTTP library for making API requests to fetch movie data.

Frontend

    HTML5: The standard markup language used to structure the web page content.
    Bootstrap: A popular CSS framework for developing responsive and mobile-first web pages.

How to use
Prerequisites

    Make sure Python 3.x is installed in your system.
    Git: If you plan to clone the repository using Git, make sure Git is installed.

How to run

    Open cmd and navigate to the directory where you want to clone the repository. Then run: git clone https://github.com/shadowking1988/Python-Project-Submission_soumalya.git
    Then use the command cd imdb-movie-scraper
    To avoid conflicts with other Python projects, create a virtual environment. Then run the following command: python -m venv venv
    This will create a virtual environment named venv in the project directory.
    To activate the virtual environment, run: venv\Scripts\activate
    Install all the necessary Python libraries using the requirements.txt file: pip install -r requirements.txt
    This will install Flask, BeautifulSoup, Requests, and other required packages.
    With the virtual environment activated, start the Flask application by running: python app.py
    This command will start the web server. You should see output indicating that the server is running, typically on http://127.0.0.1:5000/.
    Open your web browser and navigate to http://127.0.0.1:5000/. You can now use the IMDB Movie Scraper by entering a movie genre and viewing the top 25 movies for that genre.
    When you're done using the application, you can deactivate the virtual environment by simply running: deactivate

