# alx\_travel\_app

## Project Description

The **alx\_travel\_app** is a Django-based web application designed to manage travel-related listings. The application utilizes Django REST framework to build APIs, integrates MySQL for data storage, and provides API documentation via Swagger.

## Features

* User Authentication
* Create, Read, Update, Delete (CRUD) operations for travel listings
* MySQL database integration
* API documentation using Swagger
* CORS support for cross-origin requests
* Task management using Celery and RabbitMQ

## Installation

### Prerequisites

* Python 3.12+
* MySQL server
* RabbitMQ server
* Virtual environment tool (like venv)

### Clone the Repository

```bash
git clone https://github.com/username/alx_travel_app.git
cd alx_travel_app
```

### Set Up the Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Set Up Environment Variables

Create a `.env` file in the project root:

```
DATABASE_NAME=alx_travel
DATABASE_USER=root
DATABASE_PASSWORD=password
DATABASE_HOST=localhost
DATABASE_PORT=3306
```

### Run Migrations

```bash
python manage.py migrate
```

### Start the Development Server

```bash
python manage.py runserver
```

### Access API Documentation

Open your browser and go to:

```
http://127.0.0.1:8000/swagger/
```

## Running Celery

```bash
celery -A alx_travel_app worker --loglevel=info
```

