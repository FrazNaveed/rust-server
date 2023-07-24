# RUST API Server

This is an implementation of API server in RUST, which uses Actix-web, Diesel ORM & Postgres.

## ENV variables

Following are the environment variables that are required to run the API

DATABASE_URL: This is the database url of your postgres
HOST: The host of the application e.g: 127.0.0.1
PORT: The port on which the application will run. e.g: 5000

## Installation

- Clone the repo and go to the directory.
- Run the command: `diesel setup`
- Run this command to setup the migrations: `diesel migration generate`
- After setting up the migrations, run `cargo run`

## Example Request

This is the shape in which you have to give the request to the server:

{
"id": 1,
"first_name": "john",
"last_name": "doe",
"department":"Engineering",
"salary": 2350,
"age":12

}
