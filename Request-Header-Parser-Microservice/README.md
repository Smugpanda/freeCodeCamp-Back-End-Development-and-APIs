# Request Header Parser Microservice

A microservice that returns client information including IP address, preferred language, and software details.

## Description

This API service accepts HTTP requests and returns a JSON object containing the client's:
- IP Address
- Preferred Language
- Software/Browser Information

## Features

- Single endpoint that returns client information
- JSON response format
- No authentication required
- Cross-platform compatibility

## Technologies Used

- Node.js
- Express.js
- HTTP Headers Parsing

## API Endpoint

`GET /api/whoami`

### Response Format
```json
{
  "ipaddress": "159.20.14.100",
  "language": "en-US,en;q=0.5",
  "software": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:50.0) Gecko/20100101 Firefox/50.0"
}

## Live Demo
[View Live Demo](https://replit.com/@Smugpanda/boilerplate-project-headerparser/)