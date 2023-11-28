# Netflix-Clone

## Introduction

This project involves building a comprehensive Netflix clone using Django, a web framework for Python. The application will encompass various features such as user authentication, movie browsing and playback, personal watchlists, search functionality, and sections dedicated to genres and featured content.

## Features

1. **User Authentication (Signup and Login):**
   - Users can sign up by providing their email, username, and password.
   - Existing users can log in using their credentials.

2. **Browsing and Playing Movies:**
   - Users can browse through a catalog of movies.
   - Seamless playback of selected movies within the application.

3. **Adding Movies to a Personal List:**
   - Users have the ability to add movies to their personal watchlists.

4. **Search Functionality:**
   - A search feature enables users to find specific movies easily.

5. **Genres and Features Section:**
   - Dedicated sections for different genres and featured content.

## Setting Up the Project

### Prerequisites

- Python installed on your machine
- Django framework installed (`pip install django`)

### Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/samagra44/netflix-clone.git
   ```

2. **Navigate to Project Directory:**
   ```bash
   cd netflix-clone
   ```

3. **Create and Apply Migrations:**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

4. **Run the Development Server:**
   ```bash
   python manage.py runserver
   ```

5. **Access the Application:**
   Open your web browser and go to [http://localhost:8000/](http://localhost:8000/) to access the Netflix clone.

## Project Structure

The project follows a Django project structure with additional directories for templates and static files. HTML and CSS files for the Netflix clone are organized within these directories.

### Creating the URLs

Define URL patterns in the project's `urls.py` file to route requests to the appropriate views for login, signup, and homepage.

### Connecting to a Postgres Database

1. Install the required dependencies:
   ```bash
   pip install psycopg2
   ```

2. Configure the database settings in `settings.py`:
   ```python
   DATABASES = {
       'default': {
           'ENGINE': 'django.db.backends.postgresql',
           'NAME': 'your_database_name',
           'USER': 'your_username',
           'PASSWORD': 'your_password',
           'HOST': 'your_host',
           'PORT': 'your_port',
       }
   }
   ```

3. Run migrations to create necessary tables:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

### User Authentication

1. Implement a signup form to collect user details (email, username, password).
2. Validate form data, checking for existing email/username.
3. Implement a login form, authenticating users based on entered credentials.

Feel free to explore and customize the project further based on your preferences and requirements.
