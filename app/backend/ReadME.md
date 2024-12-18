# Azure OpenAI Demo - Backend

This folder contains the backend code for the Azure OpenAI demo application.

## Folder Structure

```
/C:/Users/azureuser/DemoApp/AzureOpenAIDocumentation/azure-search-openai-demo/app/backend/
├── ReadMe.md
├── app.py
├── requirements.txt
├── config/
│   ├── __init__.py
│   ├── settings.py
├── models/
│   ├── __init__.py
│   ├── model.py
├── services/
│   ├── __init__.py
│   ├── openai_service.py
├── utils/
│   ├── __init__.py
│   ├── helpers.py
└── tests/
    ├── __init__.py
    ├── test_app.py
```

## Description

This backend service is responsible for handling requests, processing data, and interacting with the OpenAI API.

## Setup

1. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

2. **Run the application**:
    ```sh
    python app.py
    ```

## Configuration

Configuration settings can be found in the `config/settings.py` file. Adjust the settings as needed for your environment.

## License

This project is licensed under the MIT License.