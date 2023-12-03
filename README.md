# Go HRMS (Human Resource Management System)

This Go project is a simple HRMS system that uses Fiber and MongoDB. It provides basic CRUD (Create, Read, Update, Delete) operations for managing employee records.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
  - [Get Employees](#get-employees)
  - [Add Employee](#add-employee)
  - [Update Employee](#update-employee)
  - [Delete Employee](#delete-employee)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Make sure you have the following tools installed:

- [Go](https://golang.org/dl/)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [Fiber](https://docs.gofiber.io/)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Mayejacob/go-hrms.git
    ```

2. Change to the project directory:

    ```bash
    cd go-hrms
    ```

3. Install dependencies:

    ```bash
    go mod download
    ```

## Configuration

Configure the project by updating the necessary settings in the `main.go` file:

```go
const dbbName = "fiber-hrms"
const mongoURI = "mongodb://localhost:27017/" + dbbName
```

## API Endpoints

- **All employee:** `GET /employee`
- **Create Employee:** `POST /employee`
- **Edit Employee:** `PUT /employee/:id`
- **Delete Employee:** `DELETE /employee/:id`

## create Employee

  ```json
        {
        "name": "John Doe",
        "salary": 50000.00,
        "age": 30
        }
    ```
    
## Update Employee

    ```json
        {
        "name": "Updated Name",
        "salary": 60000.00,
        "age": 35
        }
    ```
