# drf-cinema
Project for managing cinema using DRF

## Installing using GitHub
- Install PostgreSQL and create a database.\
- git clone https://github.com/Maytreyaya/drf-cinema
- cd drf-cinema
- python -m venv venv
- source venv/bin/activate
- pip install -r requirements.txt
- ### Setup DB
  - set POSTGRES_HOST=your_db_hostname
  - set POSTGRES_DB=your_db_name
  - set POSTGRES_USER=your_db_username
  - set POSTGRES_PASSWORD=your_db_user_password
  - set SECRET_KEY=your_secret_key


  - Apply migrations:
  python manage.py migrate
  - Start the development server:
python manage.py runserver

## Run with docker
- Docker should be installed
- docker-compose build
- docker-compose up

## Getting access
- create user via /api/user/register/
- get access token via /api/user/token/

## Features
 
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres and actors
- Creating Cinema halls
- Adding movies sessions
- Filtering movies and movie sessions