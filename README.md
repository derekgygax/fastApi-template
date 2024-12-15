# FastAPI template

This is a FastApi template that you can use when building a new FastAPI service.
It incorporates a database and general structure to follow

## MUST DO
The project contains TODO.
Search for the TODOs and do what they say to configure the project for your needs.

---

## Features - THIS IS AN EXAMPLE if it was for food

- CRUD operations for food.
- Management of storage units, and food location units, and which food animals can eat.
- Integration with a relational database (e.g., PostgreSQL).
- Role-based access control (RBAC) with JWT authentication.
- API documentation via Swagger UI and ReDoc.

---

## Requirements - example for that python version

Make sure you have the following installed:
- Python 3.12.5
- pip (Python package manager)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/derekgygax/fastApi-template.git
   cd fastApi-template
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   - Create a `.env` file in the root directory with the necessary configuration.
     Example:
     ```
     DATABASE_URL=postgresql://user:password@localhost:5432/database_name
     AUTH_SECRET=your_secret_key
     AUTH_ALGORITHM=your_algorithm
     ```

---

## Running the API

1. Start the development server:
   ```bash
   uvicorn main:app --reload
   ```


2. Access the API documentation:
   - Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
   - ReDoc: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

---

## Project Structure

```
fastApi-template/
├── app/
│   ├── models/        # Database models
│   ├── routers/        # API routes
│   ├── schemas/       # Pydantic schemas
│   ├── services/      # Business logic
│   ├── __init__.py    # Package initialization
├── main.py            # Entry point of the application
├── requirements.txt   # Dependency file
├── .env               # Environment variables
├── README.md          # Project documentation
```

---

## Testing

Run tests using your preferred testing framework (e.g., `pytest`):
```bash
pytest
```

---

## Contributing

Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request for review.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Repository

The repository for this project is hosted at: [https://github.com/derekgygax/fastApi-template.git](https://github.com/derekgygax/fastApi-template.git)
```