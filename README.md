# Late Show API

A Flask API for managing episodes, guests, and appearances on a late show.

## Setup

1. Clone the repository
2. Create a virtual environment: `python -m venv env`
3. Activate the environment:
   - Windows: `.\env\Scripts\activate`
   - Mac/Linux: `source env/bin/activate`
4. Install dependencies: `pip install -r requirements.txt`
5. Initialize the database:
   - Run migrations: `flask db init && flask db migrate && flask db upgrade`
   - Seed the database: `python seed.py`

## Running the Application

Start the server: `python app.py`

The API will be available at `http://localhost:5555`

## API Endpoints

### GET /episodes
Returns a list of all episodes

### GET /episodes/:id
Returns details of a specific episode including appearances

### GET /guests
Returns a list of all guests

### POST /appearances
Creates a new appearance with rating, episode_id, and guest_id

## Models

- **Episode**: Represents a show episode with date and number
- **Guest**: Represents a guest with name and occupation
- **Appearance**: Represents a guest appearance on an episode with a rating (1-5)