# Full Stack Chat Application

This repository contains the code for a Full Stack Chat Application built using Django Rest Framework (DRF) for the backend and ReactJS for the frontend. The application provides real-time messaging capabilities with user authentication and chat room features.

## Features

- **User Authentication**: Signup, login, and logout functionality.
- **Real-Time Messaging**: Send and receive messages in real-time.
- **Chat Rooms**: Create and join chat rooms.
- **RESTful API**: Backend built with Django Rest Framework.
- **Responsive UI**: Modern and responsive frontend built with ReactJS.

## Tech Stack

### Backend
- Django
- Django Rest Framework (DRF)
- Django Channels (for WebSocket support)
- SQLite/PostgreSQL (configurable)

### Frontend
- ReactJS
- Axios (for API requests)
- WebSocket (for real-time communication)

## Installation and Setup

### Prerequisites
- Python 3.8+
- Node.js 14+
- npm or yarn
- Virtual environment tool (e.g., `venv` or `virtualenv`)

### Backend Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Hami-611/ChatApp_FullStack.git
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

4. Run migrations:
   ```bash
   python manage.py migrate
   ```

5. Start the development server:
   ```bash
   python manage.py runserver
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   # Or if using yarn:
   yarn install
   ```

3. Start the development server:
   ```bash
   npm start
   # Or if using yarn:
   yarn start
   ```

## Folder Structure

```
fullstack-chat-app/
├── backend/
│   ├── chat/                  # Chat app logic (models, views, serializers)
│   ├── users/                 # User authentication logic
│   ├── settings.py            # Django project settings
│   └── ...
├── frontend/
│   ├── public/                # Static assets
│   ├── src/                   # React app source code
│   ├── package.json           # Frontend dependencies
│   └── ...
├── README.md                  # Project documentation
└── ...
```

## API Endpoints

### User Authentication
- **POST** `/api/auth/register/` - Register a new user
- **POST** `/api/auth/login/` - Login user
- **POST** `/api/auth/logout/` - Logout user

### Chat
- **GET** `/api/chat/rooms/` - List all chat rooms
- **POST** `/api/chat/rooms/` - Create a new chat room
- **GET** `/api/chat/rooms/{id}/messages/` - Get messages for a specific chat room
- **POST** `/api/chat/rooms/{id}/messages/` - Send a message to a chat room


## Acknowledgements

- Django Rest Framework for robust backend support.
- ReactJS for creating a responsive frontend.

Happy Coding! 🚀
