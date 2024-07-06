
# Django DRF React JWT Sample

This project is a sample implementation of a Django backend with Django Rest Framework (DRF) and a React frontend, using JSON Web Tokens (JWT) for authentication.

## Table of Contents

-   [Overview](#overview)
-   [Features](#features)
-   [Technologies Used](#technologies-used)
-   [Installation](#installation)
    -   [Backend Setup](#backend-setup)
    -   [Frontend Setup](#frontend-setup)
-   [Running the Project](#running-the-project)
-   [Project Structure](#project-structure)
-   [API Endpoints](#api-endpoints)
-   [Contributing](#contributing)
-   [License](#license)

## Overview

This repository contains a sample project demonstrating how to build a web application with Django as the backend and React as the frontend. It also shows how to implement JWT authentication using the Django Rest Framework.

## Features

-   Django backend with Django Rest Framework
-   React frontend with React Router
-   JWT authentication for secure login
-   Token refresh functionality
-   Basic CRUD operations

## Technologies Used

-   **Backend:**
    -   Django
    -   Django Rest Framework
    -   Simple JWT
-   **Frontend:**
    -   React
    -   Axios
    -   React Router

## Installation

### Backend Setup

1.  **Clone the repository:**
    
    ```
    git clone https://github.com/ZuZaaa228/djangoDRF-React-JWT-sample.git
    cd djangoDRF-React-JWT-sample/backend
    ``` 
    
2.  **Create and activate a virtual environment:**
    
    ```
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate
    ``` 
    
3.  **Install the dependencies:**
    
    ```
    pip install -r requirements.txt
    ```
    
4.  **Run migrations:**
    
    ```
    python manage.py migrate
    ```
    
5.  **Create a superuser:**
    
	   ```
   	  python manage.py createsuperuser
	   ```
    
6.  **Run the development server:**
    
    ```
    python manage.py runserver
    ```
    

### Frontend Setup

1.  **Navigate to the frontend directory:**
    
    ```
    cd ../frontend
    ```
    
2.  **Install the dependencies:**
    
    ```
    npm install
    ```
    
3.  **Start the React development server:**
    
    ```
    npm start
    ```
    

## Running the Project

After setting up both the backend and frontend, you can access the application by navigating to `http://localhost:3000` in your web browser. The backend API will be running at `http://localhost:8000`.

## Project Structure

```
djangoDRF-React-JWT-sample/
│
├── backend/
│   ├── manage.py
│   ├── myapp/
│   ├── myproject/
│   └── requirements.txt
│
└── frontend/
    ├── public/
    ├── src/
    ├── package.json
    └── README.md
```


## API Endpoints

### Authentication

-   **POST** `/api/token/` - Obtain JWT token
-   **POST** `/api/token/refresh/` - Refresh JWT token

### Users

-   **GET** `/api/users/` - List users
-   **POST** `/api/users/` - Create a new user
-   **GET** `/api/users/{id}/` - Retrieve a user
-   **PUT** `/api/users/{id}/` - Update a user
-   **DELETE** `/api/users/{id}/` - Delete a user

 [Source](https://habr.com/ru/articles/512746/) here.
