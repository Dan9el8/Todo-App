## Todo App

Todo App is a full-stack web application built with **Django** as the backend and **React** as the frontend. The project supports CRUD performance. It details the step by step procedure for creating and connecting fullstack application using django and react technologies. 



## Features

- **Create Tasks**: Add new tasks with a title, description, and due date.
- **Read Tasks**: View all your tasks in a clean and organized list.
- **Update Tasks**: Edit existing tasks to update their details.
- **Delete Tasks**: Remove tasks you no longer need.
- **Responsive Design**: The app is fully responsive and works seamlessly on all devices.



## Technologies Used

### Backend (Django)
- **Django**: A high-level Python web framework for building robust APIs.
- **Django REST Framework (DRF)**: For creating RESTful APIs.
- **CORS Headers**: To handle cross-origin requests between the frontend and backend.


### Frontend (React)
- **React**: A JavaScript library for building user interfaces.
- **Axios**: For making HTTP requests to the Django backend.
- **React Router**: For handling navigation within the app.
- **Bootstrap**: For styling and responsive design.



## Prerequisites

Before you begin, ensure you have the following installed:

- **Python 3.x**: For running the Django backend.
- **Node.js**: For running the React frontend.
- **pip**: Python package installer.
- **npm**: Node package manager.



## Setup Instructions

### Backend (Django)

1. **Clone the repository**:
   git clone https://github.com/your-username/todo-project.git
   cd todo-project/backend
   

2. **Create a virtual environment**:
      python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   

3. **Install dependencies**:
   pip install -r requirements.txt
   

4. **Apply migrations**:
   python manage.py migrate
   

5. **Run the Django server**:
   python manage.py runserver
   
   The backend will be available at `http://127.0.0.1:8000`.

### Frontend (React)

1. **Navigate to the frontend directory**:
   
   cd ../frontend
   
2. **Install dependencies**:
   
   npm install
   

3. **Run the React development server**:
   
   npm start
   
   The frontend will be available at `http://localhost:3000`.

---

## Project Structure

```
Todo App/
├── todobackend/                  # Django backend
│   ├── api/                 # Django app for the TODO functionality
│   ├── manage.py             # Django management script
│   └── requirements.txt      # Python dependencies
├── frontend/                 # React frontend
│   ├── public/               # Static assets
│   ├── src/                  # React components and logic
│   └── package.json          # Node.js dependencies
└── README.md                 # This file
```

---

## API Endpoints

The Django backend exposes the following RESTful API endpoints:

- **GET /api/tasks/**: Retrieve all tasks.
- **POST /api/tasks/**: Create a new task.
- **GET /api/tasks/<id>/**: Retrieve a specific task by ID.
- **PUT /api/tasks/<id>/**: Update a specific task by ID.
- **DELETE /api/tasks/<id>/**: Delete a specific task by ID.

## CORS Configuration

CORS (Cross-Origin Resource Sharing) is configured in the Django backend to allow requests from the React frontend. This is done using the `django-cors-headers` package. The following settings are added to `settings.py`:

```python
INSTALLED_APPS = [
    ...
    'corsheaders',
    ...
]

MIDDLEWARE = [
    ...
    'corsheaders.middleware.CorsMiddleware',
    ...
]

CORS_ALLOWED_ORIGINS = [
    "http://localhost:3000",  # React frontend URL
]

## Contributing

Contributions are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Push your branch and submit a pull request.



## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or feedback, feel free to reach out:

- **Email**: mutetemifloice@gmail.com