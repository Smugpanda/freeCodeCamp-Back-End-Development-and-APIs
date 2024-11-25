# URL Shortener Microservice

A RESTful API service that creates shortened URLs from long URLs, similar to bit.ly or TinyURL.

## Description

This microservice allows users to:
- Submit a URL for shortening
- Receive a unique short URL identifier
- Use the short URL to redirect to the original URL

## Features

- URL validation
- Unique short URL generation
- Permanent URL storage
- Redirect functionality
- Error handling for invalid URLs

## Technologies Used

- Node.js
- Express.js
- MongoDB
- DNS lookup validation

## API Endpoints

### POST /api/shorturl
Creates a short URL from a provided URL

**Request Format:**
```json
{
  "url": "https://www.google.com"
}

## Live Demo
[View Live Demo](https://boilerplate-project-urlshortener.smugpanda.repl.co/)