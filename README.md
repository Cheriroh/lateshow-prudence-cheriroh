# Late Show Flask API

This project is a Flask-based RESTful API that manages episodes, guests, and guest appearances on the Late Show. It supports viewing episodes, managing guests, and recording guest appearances with ratings.


## Features

- View all Late Show episodes
- View specific episode by ID
- View all guests
- Add a guest appearance with a rating (1–5)
- Validations and error handling
- Cascade deletes for related appearances
- Seed database from CSV file


## Tech Stack

- Python 3.10+
- Flask
- Flask-SQLAlchemy
- Flask-Migrate
- SQLite (for development)
- Postman (for API testing)


## Setup Instructions

### 1. Clone the Repository

```
git clone https://github.com/Cheriroh/lateshow-prudence-cheriroh
cd lateshow
2. Create a Virtual Environment
3. Install Dependencies
pip install Flask Flask-SQLAlchemy Flask-Migrate
```
4. Set Up the Database

flask db init
flask db migrate -m "Initial migration."
flask db upgrade

5. Seed the Database
Make sure seed.csv is present in the root folder. Then:

python seed.py

Running the App

python app.py

By default, the app runs on: http://127.0.0.1:5000

API Endpoints
 Episodes
GET /episodes
Returns all episodes.

GET /episodes/<id>
Returns one episode with its guest appearances.

 Guests
GET /guests
Returns all guests.

 Appearances
POST /appearances
Create a new appearance. JSON Body:

## Contributing
* Fork the repository

* Create a new branch

* Commit your changes

* Open a pull request

## Author
Prudece Chepkorir
Flask | SQLAlchemy | REST APIs

## License
Copyright (c) 2025 PRUDENCE CHEPKORIR

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
