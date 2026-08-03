# CRUD API

This project is a simple CRUD (Create, Read, Update, Delete) REST API built using FastAPI as part of the FlyRank Backend Assignment. The API stores tasks in memory and allows users to create, view, update, and delete tasks through HTTP endpoints.

## Features

* Create a new task
* View all tasks
* View a task by its ID
* Update an existing task
* Delete a task
* Interactive API documentation with Swagger UI

## Technologies Used

* Python 3
* FastAPI
* Pydantic
* Uvicorn

## Getting Started

### Clone the repository

```bash
git clone https://github.com/AbdulHadi638/flyrank_crud_task-api.git
cd flyrank_crud_task-api
```

### Install dependencies
pip install fastapi uvicorn
```

### Run the server
py -m uvicorn main:app --reload
```

Once the server starts, open:

* API: http://localhost:8000
* Swagger UI: http://localhost:8000/docs

## API Endpoints

| Method | Endpoint    |  Purpose               |
| ------ | ----------- | ----------------------- |
| GET   |  /          | API information          |  
| GET    | /health     | Health check            |
| GET     | /tasks      | Get all tasks           |
| GET    | /tasks/{id} | Get a task by ID        |
| POST   | /tasks     | Create a new task       |
| PUT    | /tasks/{id} | Update an existing task |
| DELETE | /tasks/{id} | Delete a task           |

## Example curl Request

curl -i -X POST http://localhost:8000/tasks ^ -H "Content-Type: application/json" ^ -d "{\"title\":\"Buy milk\"}"

## Swagger UI
[Swagger UI](swagger.png)



## Author

Abdul Hadi
