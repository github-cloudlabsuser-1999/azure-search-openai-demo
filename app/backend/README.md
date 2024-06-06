# Backend Application

The backend application is built using [Quart](https://quart.palletsprojects.com/), a Python framework for asynchronous web applications. The backend code is stored in the `app/backend` folder.

## Getting Started

To start the backend application, you can use the `start.ps1` script located in the `app` directory. This script installs the necessary Python and npm packages and starts the backend server.

## Directory Structure

- `approaches/`: Contains the classes powering the Chat and Ask tabs. Each class uses a different RAG (Retrieval Augmented Generation) approach.
- `prepdocs.py`: Sets up file processors for different file types.

## Key Files

- `approach.py`: Defines the `Approach` abstract base class and the `Document` and `ThoughtStep` data classes.
- `prepdocs.py`: Defines the `setup_file_processors` function, which sets up file processors for different file types.

## Running the Application

To run the backend application, navigate to the `app/backend` directory and run the following command:

```sh
python3 -m gunicorn main:app

Customization
You can customize the backend application by modifying the classes in the approaches directory. For more information on customization, see the customization guide.

Contributing
Please see the CONTRIBUTING.md file for details on how to contribute to the backend application.

License
This project is licensed under the terms of the license provided in the LICENSE file.