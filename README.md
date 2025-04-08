# Flask API Hello

This project is a simple Flask-based API that returns a "Hello, World!" response. It is containerized using Docker for easy deployment.

## Features

- Lightweight Flask application.
- Dockerized for portability and scalability.
- Simple "Hello, World!" endpoint.

## Requirements

- Python 3.8+
- Docker (optional for containerized deployment)

## Installation

1. Clone the repository:
  ```bash
  git clone https://github.com/your-repo/flask-api-hello.git
  cd flask-api-hello
  ```

2. Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```

3. Run the application:
  ```bash
  python app.py
  ```

## Usage

The application exposes a single endpoint:

- `GET /` - Returns "Hello, World!".

Example:
```bash
curl http://127.0.0.1:5000/
```

## Docker Deployment

1. Build the Docker image:
  ```bash
  docker build -t flask-api-hello .
  ```

2. Run the container:
  ```bash
  docker run -p 5000:5000 flask-api-hello
  ```

3. Access the API:
  ```bash
  curl http://127.0.0.1:5000/
  ```

## File Structure

- `app.py`: Main Flask application.
- `Dockerfile`: Instructions to build the Docker image.
- `requirements.txt`: Python dependencies.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.