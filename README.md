# File Metadata Microservice for FCC

This is a file metadata microservice project for freeCodeCamp.

## Objective

The objective of this project is to create an API endpoint that accepts a file upload and returns metadata about the uploaded file, such as the file name, size, and MIME type.

## API Endpoint

- **POST /upload** - Uploads a file and returns its metadata.

### Request

- Method: `POST`
- Endpoint: `/upload`
- Headers: `Content-Type: multipart/form-data`
- Body:
  - Key: `upfile`
  - Value: File

### Response

The API will respond with a JSON object containing the following metadata of the uploaded file:

```json
{
  "name": "example.txt",
  "size": 12345,
  "mimetype": "text/plain"
}
