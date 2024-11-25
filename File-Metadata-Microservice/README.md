# File Metadata Microservice

A simple API service that analyzes uploaded files and returns their metadata information.

## Description

This microservice allows users to:
- Upload files through a simple web interface
- Receive metadata about the uploaded file
- Handle multiple file types securely

## Features

- File upload functionality
- Metadata extraction
- Secure file handling
- Multiple file type support
- User-friendly interface

## Technologies Used

- Node.js
- Express.js
- Multer (for file handling)
- HTML/CSS (for upload interface)

## API Endpoint

### POST /api/fileanalyse
Analyzes uploaded file and returns metadata

**Response Format:**
```json
{
  "name": "example.txt",
  "type": "text/plain",
  "size": 12345
}

## Live Demo
[View Live Demo](https://boilerplate-project-filemetadata.smugpanda.repl.co/)
