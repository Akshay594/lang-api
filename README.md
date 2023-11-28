
# Flask Translation API

This project is a simple Flask-based web application providing a translation service. It utilizes Google's unofficial translation API to translate text from one language to another and detect the source language. The API also supports the removal of diacritics from the translated text. Swagger UI is integrated for easy testing and documentation of the API endpoints.

## Features

- Translation of text to specified target language.
- Detection of the source language of the text.
- Removal of diacritics from the translated text.
- Swagger UI for interactive API documentation and testing.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3
- Flask
- Flask-CORS
- Flask-RESTx
- Googletrans

### Installation

Clone the repository:

```bash
git clone [URL_of_Your_Repository]
cd [Your_Repository_Name]
```

Install the required packages:

```bash
pip install -r requirements.txt
```

### Running the Application

Run the application locally:

```bash
python app.py
```

The application will be available at `http://localhost:8000/`. The Swagger UI can be accessed at the root URL for testing the API.

## Usage

The API provides the following endpoints:

- `GET /`: A simple endpoint to check if the API is running.
- `POST /translate/`: Endpoint to translate text. It accepts JSON data with the following structure:

  ```json
  {
      "input_text": "Hello, World!",
      "dest": "es"
  }
  ```

## Contributing

Contributions to this project are welcome. Please ensure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Contact

Your Name - gopalsinghpanwar411@gmail.com

# Adding Zappa with AWS Lambda production instructions to the README.md content

## Deploying to AWS Lambda with Zappa

This application can be deployed to AWS Lambda using Zappa, which makes it easy to build and deploy serverless Python applications.

### Prerequisites for AWS Lambda Deployment

- An AWS account with appropriate permissions.
- AWS CLI installed and configured.
- Zappa installed (`pip install zappa`).

### Zappa Configuration

1. **Initialize Zappa:** Run `zappa init` in the project directory. This will guide you through creating a `zappa_settings.json` file.

2. **Customize `zappa_settings.json`:** Modify the generated `zappa_settings.json` file as needed for your deployment settings.

### Deployment

1. **Deploy with Zappa:** Run `zappa deploy` to deploy your application to AWS Lambda.

2. **Update the Application:** If you make changes, use `zappa update` to update the application on AWS Lambda.

3. **Access the Application:** Once deployed, Zappa will provide you with a URL to access your application.

### Additional Zappa Commands

- **Rollback:** To rollback to a previous version, use `zappa rollback`.
- **Monitoring:** Use `zappa status` to monitor the status of your deployment.
- **Undeploy:** Use `zappa undeploy` to remove the application from AWS Lambda.

For more information on Zappa and its commands, visit the [Zappa GitHub repository](https://github.com/Miserlou/Zappa).
"""
