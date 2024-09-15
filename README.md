
---

# Task List Application

![Stack](https://img.shields.io/badge/stack-PostgreSQL%20%7C%20Python%20%7C%20Gunicorn%20%7C%20Nginx%20%7C%20Docker-blue)

## Description

This is a simple task list application that allows users to:

- Add tasks
- Remove tasks
- Mark tasks as completed

The project is designed for educational purposes to demonstrate basic concepts and configurations using Docker, PostgreSQL, Python, and Nginx.

## Technologies Used

- **PostgreSQL**: Database system for storing tasks.
- **Python**: Backend language used to manage tasks.
- **Gunicorn**: WSGI HTTP server for Python applications.
- **Nginx**: Web server used as a reverse proxy for the application.
- **Docker**: Containerization platform used to manage application deployment.

## Getting Started

To get started with the project, follow these steps:

1. **Clone the Repository**

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Build and Start the Containers**

   ```bash
   docker-compose up --build
   ```

3. **Access the Application**

   Open your web browser and navigate to `http://localhost` to access the task list application.

## Environment Variables

**Warning**: The environment variables provided in this project are for development purposes only and should not be used in a production environment. Make sure to use secure and appropriate values for environment variables in a production setup.

## File Structure

```
.
├── backend
│   ├── app.py
│   ├── Dockerfile
│   ├── requirements.txt
│   └── wsgi.py
├── database
│   ├── Dockerfile
│   └── init_db.sh
├── docker-compose.yaml
├── frontend
│   ├── Dockerfile
│   ├── nginx
│   │   ├── nginx
│   │   │   └── nginx.conf
│   │   └── nginx.conf
│   └── todo-list
│       ├── package.json
│       ├── public
│       │   ├── index.html
│       │   ├── manifest.json
│       │   └── robots.txt
│       ├── src
│       │   ├── api.ts
│       │   ├── App.tsx
│       │   ├── DeskFooter
│       │   │   ├── DeskFooter.css
│       │   │   └── DeskFooter.tsx
│       │   ├── index.css
│       │   ├── index.tsx
│       │   ├── InputField
│       │   │   ├── InputField.css
│       │   │   └── InputField.tsx
│       │   ├── TaskDesk
│       │   │   ├── TaskDesk.css
│       │   │   └── TaskDesk.tsx
│       │   ├── TaskItem
│       │   │   ├── TaskItem.css
│       │   │   └── TaskItem.tsx
│       │   ├── Title
│       │   │   ├── Title.css
│       │   │   └── Title.tsx
│       │   └── types.ts
│       └── tsconfig.json
├── nginx
│   └── nginx.conf
└── README.md

```
---
 
## License

This project is intended for educational purposes only and is not licensed for commercial use.

---

Feel free to adjust any sections as needed!
