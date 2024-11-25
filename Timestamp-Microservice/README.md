# Timestamp Microservice

## Description

This microservice accepts a date string as input and returns a JSON object with both Unix and UTC timestamps.

## Features

1. Accepts valid date strings or Unix timestamps via URL parameters.
2. Returns a JSON object with:
    - `unix`: Unix timestamp.
    - `utc`: Human-readable UTC timestamp.

## Technologies Used

- Node.js
- Express.js

## How to Use

1. Clone this repository:
    ```bash
    git clone <https://github.com/smugpanda/freeCodeCamp-Back-End-Development-and-APIs.git>
    cd Timestamp-Microservice
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Start the server:
    ```bash
    npm start
    ```

4. Use the following endpoints:
    - `/api/:date?` - Returns timestamps for a given date or current date if no input is provided.

## Example Usage

1. `/api/2015-12-25` returns:
    ```json
    {
      "unix": 1451001600000,
      "utc": "Fri, 25 Dec 2015 00:00:00 GMT"
    }
    ```

2. `/api/1451001600000` returns:
    ```json
    {
      "unix": 1451001600000,
      "utc": "Fri, 25 Dec 2015 00:00:00 GMT"
    }
    ```

## Live Demo
[View Live Demo](https://boilerplate-project-timestamp.smugpanda.repl.co/)
