# FastAPI Application

This project is a simple REST API built with FastAPI for managing items. It demonstrates how to create, retrieve, update, and delete items using FastAPI endpoints.

## Table of Contents

1. [Project Setup](#project-setup)
2. [Endpoints](#endpoints)
3. [Running the Project](#running-the-project)
4. [Testing](#testing)
5. [Contributing](#contributing)
6. [License](#license)

## Project Setup

### Prerequisites

- **Python** 3.7+
- **FastAPI** (for API framework)
- **Uvicorn** (ASGI server)

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repo-url>
   cd <repo-name>
   ```

2. **Install dependencies**:
   ```bash
   pip install fastapi uvicorn
   ```

## Endpoints

The API includes the following endpoints for managing items:

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | / | Welcome message |
| GET | /items/{item_id} | Retrieve an item by ID |
| POST | /items | Create a new item |
| PUT | /items/{item_id} | Update an existing item |
| DELETE | /items/{item_id} | Delete an item by ID |

### Sample JSON for POST/PUT Requests

To create or update an item, send JSON data in the following format:

```json
{
  "name": "Sample Item",
  "description": "This is a sample item.",
  "price": 10.99,
  "tax": 0.50
}
```

## Running the Project

To start the FastAPI application:

1. Run the server with Uvicorn:
   ```bash
   uvicorn main:app --reload
   ```

2. Visit http://127.0.0.1:8000/docs to explore the API using the automatically generated Swagger UI.

## Testing

You can run tests for the application by using the following command:

```bash
pytest
```

Ensure that you have installed pytest if it's not already in your development environment.

## Contributing

We welcome contributions to this project. To contribute:

1. **Fork the repository**

2. **Create a feature branch**:
   ```bash
   git checkout -b feature/NewFeature
   ```

3. **Commit your changes**:
   ```bash
   git commit -m 'Add NewFeature'
   ```

4. **Push to the branch**:
   ```bash
   git push origin feature/NewFeature
   ```

5. **Open a Pull Request**

## License

This project is licensed under the MIT License.