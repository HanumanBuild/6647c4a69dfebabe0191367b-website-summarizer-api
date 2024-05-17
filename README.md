# Website Summarizer API

## Overview
This API takes in a website URL, fetches the content, and uses OpenAI to summarize the contents of the page. The summarized content is then stored in a MongoDB database.

## Endpoint

### POST /summarize
- **Description:** Summarizes the content of the given URL.
- **Request Body:**
  ```json
  {
    "url": "https://example.com"
  }
  ```
- **Response:**
  ```json
  {
    "url": "https://example.com",
    "summary": "This is a summary of the content.",
    "createdAt": "2023-10-01T00:00:00.000Z"
  }
  ```

## Setup
1. Clone the repository.
2. Install dependencies: `npm install`
3. Start the server: `node server.js`
