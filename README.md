# demo-fullstack



## Install

`yarn`

## DB Setup

Copy .env.example to .env and set `DATABASE_URL` and `PORT` to your liking.

Example for a local database: `DATABASE_URL=postgres://neill@localhost/pastebin`

You will need to create your own databases for this project - one locally and one on Heroku.

## Running locally

`yarn start:dev`

This will set the env var LOCAL to true, which will cause the db connection configuration to NOT use SSL (appropriate for your local db)

## running on heroku

When the project is deployed to heroku, the command in your `Procfile` file will be run.

Heroku will itself supply the env var `DATABASE_URL` and the given server code will connect based on that connection string.
