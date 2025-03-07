To create a well-documented README.md file for your API, follow these steps:


# Task Management API

This is a simple Task Management API built using Node.js and Express. It allows users to create, retrieve, update, and delete tasks. Users can also filter tasks by priority and completion status.

 List Setup Instructions
Provide step-by-step instructions for setting up and running the API.


## API Endpoints
**Endpoint:**  


1.GET /tasks
Query Parameters (Optional):


[
  {
    "id": 1,
    "title": "Create a new project",
    "description": "Create a new project using Magic",
    "completed": false,
    "priority": "medium",
    "createdAt": "2024-03-04T12:00:00Z"
  }
]


2. Get Task by ID
Endpoint:

GET /tasks/:id
Response:

{
  "id": 1,
  "title": "Create a new project",
  "description": "Create a new project using Magic",
  "completed": false,
  "priority": "medium",
  "createdAt": "2024-03-04T12:00:00Z"
}


3. Create a New Task
Endpoint:

POST /tasks
{
  "title": "New Task",
  "description": "Task description",
  "completed": false,
  "priority": "high"
}
Response:


{
  "id": 2,
  "title": "New Task",
  "description": "Task description",
  "completed": false,
  "priority": "high",
  "createdAt": "2024-03-04T12:05:00Z"
}


4. Update a Task

PUT /tasks/:id
t
{
  "title": "Updated Task",
  "description": "Updated description",
  "completed": true
}
Response:

{
  "id": 2,
  "title": "Updated Task",
  "description": "Updated description",
  "completed": true,
  "priority": "high",
  "createdAt": "2024-03-04T12:05:00Z"
}


5. Delete a Task
Endpoint:

DELETE /tasks/:id
Response:

{
  "message": "Task deleted successfully"
}


## Testing the API

### Using Postman
1. Open Postman.
2. Enter `http://localhost:3000/tasks` in the request URL.
3. Select the appropriate HTTP method (GET, POST, PUT, DELETE).
4. If required, add a request body in JSON format.
5. Click **Send** to see the response.

