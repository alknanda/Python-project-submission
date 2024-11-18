IMDB Movie Scraper

IMDB Movie Scraper is a web application built with Flask that allows users to search for movies by genre. The application scrapes movie data from IMDB and displays the top 25 movies for the specified genre, including the title, year, rating, and metascore.
Project Structure

    app.py: The main Python file that contains the backend logic for the web application.
    templates/index.html: The HTML file that serves as the frontend of the application, rendered by Flask.

Code Explanation
Python Code: app.py

app.py is the backend of the IMDB Movie Scraper application. Below is a breakdown of the key sections of the code:

    Imports:
        Flask: The web framework used to create the application.
        render_template: Renders HTML templates.
        request: Handles form data submitted by the user.
        flash: Displays messages to the user.
        requests: Sends HTTP requests to IMDB.
        BeautifulSoup: Parses HTML and extracts data from web pages.

    Flask Application Instance:
        app = Flask(__name__): Initializes the Flask application.
        app.secret_key: Sets a secret key required for session management and flashing messages.

    Movie Scraping Function (scrape_movies_by_genre):
        Constructs the IMDB URL for the specified genre.
        Sends an HTTP request to fetch the search results.
        Uses BeautifulSoup to parse the HTML and extract movie details such as title, year, rating, and metascore.
        Handles pagination to collect up to 25 movies.

    Flask Route:
        The main route ("/") handles both GET and POST requests.
        When a genre is submitted, the route calls scrape_movies_by_genre to fetch movie data.
        The results are then passed to the index.html template for rendering.

HTML Code: index.html

index.html is the frontend of the application. Here's how it works:

    Head Section:
        Defines the page's metadata and links to the Bootstrap CSS framework for styling.
        Includes a JavaScript function that allows the form to be submitted by pressing the Enter key.

    Body Section:
        Displays a search form where users can input a movie genre.
        If movies are found, they are displayed in a Bootstrap-styled table.
        Error messages are displayed using Bootstrap's alert system.

    Movie Display:
        The movie data passed from Flask is dynamically rendered in the table.
        The title on the results page reflects the genre searched by the user (e.g., "Top 25 Action Movies").

Interaction Between app.py and index.html

    User Input: The user enters a movie genre and submits the form.
    Backend Processing: The Flask server processes the input, scrapes IMDB for the top 25 movies in that genre, and passes the data to the template.
    Rendering: The index.html template displays the results in a clean and responsive format.

