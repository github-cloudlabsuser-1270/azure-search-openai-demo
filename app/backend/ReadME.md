# Azure OpenAI Demo - Backend

This folder contains the backend code for the Azure OpenAI demo application.

## Overview

The backend application is built using [Quart](https://quart.palletsprojects.com/), a Python framework for asynchronous web applications. It handles various functionalities such as handling chat and ask requests, file uploads, and integration with Azure services.

## Folder Structure

├── ReadMe.md ├── app.py ├── requirements.txt ├── config.py ├── auth.py ├── helpers.py ├── approaches/ │ ├── chatreadretrieveread.py │ ├── retrievethenread.py │ ├── chatreadretrievereadvision.py │ ├── retrievethenreadvision.py │ └── ... └── ...

## Key Files and Their Functionalities

### [app.py](app.py)

- Sets up the Quart application.
- Defines routes and configures various services like Azure Blob Storage, Azure OpenAI, and authentication.
- Key routes include:
  - `/ask`: Handles requests to ask questions.
  - `/chat`: Handles chat requests.
  - `/upload`: Handles file uploads.
  - `/delete_uploaded`: Handles deletion of uploaded files.
  - `/list_uploaded`: Lists uploaded files.

### [approaches/](approaches/)

- Contains different approaches for handling chat and ask functionalities.
- Examples include:
  - [`chatreadretrieveread.py`](approaches/chatreadretrieveread.py)
  - [`retrievethenread.py`](approaches/retrievethenread.py)
  - [`chatreadretrievereadvision.py`](approaches/chatreadretrievereadvision.py)
  - [`retrievethenreadvision.py`](approaches/retrievethenreadvision.py)

### [auth.py](auth.py)

- Contains authentication helpers and decorators to secure routes and manage user sessions.

### [config.py](config.py)

- Manages backend configuration using environment variables and constants.

### [helpers.py](helpers.py)

- Contains helper functions used across the backend application.

## Configuration

The backend configuration is managed using environment variables. Key configurations include:

- `AZURE_STORAGE_ACCOUNT_NAME`
- `AZURE_STORAGE_ACCOUNT_KEY`
- `AZURE_OPENAI_API_KEY`
- `AZURE_OPENAI_ENDPOINT`
- `AZURE_SEARCH_SERVICE_NAME`
- `AZURE_SEARCH_INDEX_NAME`

## Error Handling

The backend includes error handling mechanisms to log and respond to errors appropriately.

## Running the Backend

To run the backend application locally, use the following command:

```sh
quart run