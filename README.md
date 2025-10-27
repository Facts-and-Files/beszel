# Dockerized Beszel

## Building for development/local docker

There is an .env.example file.
Make your changes there and rename it to .env
The start the image.

    $ docker compose up -d

When started the first time browse to the Hub at http://localhost:8090 and create a token and a key. 

Then stop the container:

    $ docker compose down

Add these to you .env and rebuild/restart the conainer:

    $ docker compose up -d --build --force-recreate

For further documentation see the official guide at https://beszel.dev/.

## Deployment

Deployment is done by Github actions.

