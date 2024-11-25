# Exercise Tracker API

A RESTful API service that allows users to track their exercise activities and retrieve their exercise logs.

## Description

This microservice enables users to:
- Create a new user account
- Log exercises with duration and date
- Retrieve complete exercise logs
- Filter logs by date range and limit

## Features

- User registration
- Exercise logging
- Date-based filtering
- Limit query support
- Comprehensive exercise history

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Date handling

## API Endpoints

### POST /api/users
Creates a new user

**Response Format:**
```json
{
  "username": "fcc_test",
  "_id": "5fb5853f734231456ccb3b05"
}

POST /api/users/:_id/exercises
Adds an exercise for user
Request Format: json
{
  "description": "running",
  "duration": 30,
  "date": "2024-01-01"
}

GET /api/users/:_id/logs
Retrieves exercise logs
Query Parameters:
from (date)
to (date)
limit (number)
Response Format:
json
{
  "username": "fcc_test",
  "count": 1,
  "log": [{
    "description": "running",
    "duration": 30,
    "date": "Mon Jan 01 2024"
  }]
}

Setup
Clone the repository:
bash
git clone <your-repository-url>
cd Exercise-Tracker

Install dependencies:
bash
npm install

Start the server:
bash
npm start

Example Usage
Create new user:
text
POST /api/users
Response: {"username": "user1", "_id": "5fb5853f734231456ccb3b05"}

Log exercise:
text
POST /api/users/5fb5853f734231456ccb3b05/exercises
Body: {"description": "running", "duration": 30, "date": "2024-01-01"}

Get logs:
text
GET /api/users/5fb5853f734231456ccb3b05/logs?from=2024-01-01&to=2024-12-31&limit=10

## Live Demo
[View Live Demo](https://boilerplate-project-exercisetracker.smugpanda.repl.co/)