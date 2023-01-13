# dockerize-cinema-order-tickets-service

API service for cinema management written on DRF

# Installing using GitHub

install PostgresSQL and create db

    git clone https://github.com/maxitoska/dockerize-cinema-order-tickets-service.git
    python -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    set POSTGRES_HOST=<your POSTGRES hostname>
    set POSTGRES_NAME=<your POSTGRES name>
    set POSTGRES_USER=<your POSTGRES username>
    set POSTGRES_PASSWORD=<your POSTGRES user password>
    set SECRET_KEY=<your secret key>
    python manage.py migrate
    python manage.py runserver

# Run with docker

Docker should be installed
    
    docker-compose build
    docker-compose up

# Getting access

create user via /api/user/register/
get access token via /api/user/token/
refresh token via /api/user/token/refresh/
