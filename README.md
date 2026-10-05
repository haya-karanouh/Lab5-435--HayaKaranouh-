# Lab 5 – Postman and APIs

This project is a Flask REST API using SQLite for simple user management. It is designed for the EECE 435 lab and demonstrates creating, reading, updating, and deleting data through HTTP requests tested with Postman.

## Project Structure

- app.py
- database.py
- database.db
- requirements.txt
- Flask_user_app.postman_collection.json
- screenshots/

## Setup Instructions

Create a virtual environment:

```bash
python -m venv venv
```

Activate it on macOS/Linux:

```bash
source venv/bin/activate
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the app:

```bash
python app.py
```

The application runs at http://localhost:5000

## API Endpoints

| Method | Endpoint | Description |
| --- | --- | --- |
| GET | /api/users | Get all users |
| GET | /api/users/<user_id> | Get one user |
| POST | /api/users/add | Add a user |
| PUT | /api/users/update | Update an entire user |
| PATCH | /api/users/<user_id> | Partially update a user |
| DELETE | /api/users/delete/<user_id> | Delete a user |

## Postman Setup

1. Open Postman.
2. Import Flask_user_app.postman_collection.json.
3. Create a Postman environment.
4. Add the variable:
   - base_url = http://localhost:5000
5. Select the environment.
6. Run the requests in order.

## Screenshots

The required screenshots for the successful API requests are stored in the screenshots/ folder.
