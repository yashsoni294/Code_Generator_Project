# Code Generator Backend Tool

Welcome to the Code Generator Backend Tool! This project provides a backend service that generates code based on specified templates and configurations. This README will guide you through setting up the environment, installing dependencies, and running the application.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.12.8 or higher
- pip (Python package installer)
- Virtual environment (optional but recommended)

## Setup Instructions

1. **Create a new virtual environment**:

   ```bash
   python3 -m venv myenv
   ```

2. **Activate the virtual environment**:

   - On Windows:
     ```bash
     myenv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source myenv/bin/activate
     ```

3. **Install dependencies**:

   Install all required packages by running the following command:

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

Before running the application, you need to configure the environment variables in the `.env` file. Update the following paths according to your server setup:

```plaintext
FRONTEND_BASE_FOLDER = /path/to/frontend
TEST_CASES_BASE_FOLDER = /path/to/test_cases
BACKEND_BASE_FOLDER = /path/to/backend
```

Make sure to replace `/path/to/...` with the actual paths on your server.

## Running the Application

Once you have configured the environment variables, you can start the application using Uvicorn. Run the following command:

```bash
uvicorn main:app --reload
```

The `--reload` flag enables auto-reload, which is useful during development as it automatically restarts the server when code changes are detected.

## Usage

After starting the application, you can access the API at `http://127.0.0.1:8000`. You can use tools like Postman or curl to interact with the API endpoints.

## Contributing

We welcome contributions to this project! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for using the Code Generator Backend Tool! If you have any questions or issues, feel free to reach out. Happy coding!
