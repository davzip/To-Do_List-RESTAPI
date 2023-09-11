# Baby Tracker REST API

## Overview

This project is a REST API for tracking baby-related events. It consists of both a backend and a frontend component.

### Backend

#### Technologies Used
- **Flask**: A micro web framework for Python used for building the REST API.
- **SQLAlchemy**: An SQL toolkit and Object-Relational Mapping (ORM) library for Python used to interact with the PostgreSQL database.
- **PostgreSQL**: A powerful open-source relational database management system.
- **Flask-CORS**: An extension for handling Cross-Origin Resource Sharing (CORS) in Flask applications.

#### Purpose
The backend of this project serves as the core component for managing baby-related events. It provides the following functionalities:

1. **Create Event**: POST request to `/events` allows users to create a new baby-related event. The event description is provided in the request body.

2. **Get All Events**: GET request to `/events` retrieves a list of all baby-related events. Events are sorted by their creation date in ascending order.

3. **Get Single Event**: GET request to `/events/<id>` retrieves a single baby-related event based on its unique identifier (id).

4. **Update Event**: PUT request to `/events/<id>` allows users to update an existing event. The event description can be modified in the request body.

5. **Delete Event**: DELETE request to `/events/<id>` allows users to delete a specific event by providing its unique identifier (id).

### Frontend

#### Technologies Used
- **React**: A popular JavaScript library for building user interfaces.
- **Axios**: A promise-based HTTP client for making requests to the backend API.
- **date-fns**: A JavaScript date utility library used for formatting dates.

#### Purpose
The frontend of this project is a user interface that interacts with the backend API to enable users to track and manage baby-related events. It provides the following features:

1. **Create Event**: Users can enter a description of the event and submit it to create a new event.

2. **Edit Event**: Users can edit an existing event by clicking the "Edit" button next to it. This allows them to modify the event description.

3. **Delete Event**: Users can delete an event by clicking the "X" button next to it.

4. **List Events**: All events are listed in a chronological order, displaying their creation date and description.

## How to Run the Project

1. Clone this repository to your local machine.

2. Start the backend server:
   - Make sure you have Python and PostgreSQL installed.
   - Navigate to the backend directory.
   - Install the required Python packages using `pip install -r requirements.txt`.
   - Update the database URI in `app.config['SQLALCHEMY_DATABASE_URI']` to match your PostgreSQL configuration.
   - Run the Flask application using `python app.py`.

3. Start the frontend application:
   - Navigate to the frontend directory.
   - Install the required Node.js packages using `npm install`.
   - Start the React application using `npm start`.

4. Access the application in your web browser at `http://localhost:3000`.

You can now use the Baby Tracker to record and manage baby-related events!
