# TeamTask API

A robust, scalable, and real-time backend API for a collaborative task management application built with Django REST Framework.

## 🚀 Features

- **JWT Authentication:** Secure login and refresh tokens.
- **Workspace & Team Collaboration:** Create workspaces and invite team members.
- **Boards, Lists, and Tasks:** Full CRUD functionality with nested relationships.
- **Advanced Permissions:** Fine-grained controls ensuring users only access what they are allowed to.
- **Real-time Updates:** Live updates for tasks and boards using WebSockets (Django Channels).
- **Comprehensive Documentation:** Full API documentation generated using OpenAPI (Swagger).
- **Test Suite:** High test coverage with Pytest.
- **Dockerized:** Containerized for easy development and deployment.
- **CI/CD:** Automated testing with GitHub Actions.

## 🛠️ Tech Stack

- **Django 4.2+**
- **Django REST Framework**
- **Django Channels** (WebSockets)
- **PostgreSQL**
- **Redis** (Channel layer)
- **SimpleJWT** (Authentication)
- **Docker & Docker-compose**
- **Pytest** (Testing)
- **DRF Spectacular** (Documentation)

## 📚 API Documentation

Once the server is running, access the interactive API documentation:
- Swagger UI: `/api/schema/swagger-ui/`
- ReDoc: `/api/schema/redoc/`

## 🏁 Getting Started

### Prerequisites
- Docker and Docker-compose

### Installation
1.  Clone the repository:
    ```bash
    git clone https://github.com/yourusername/teamtask-api.git
    cd teamtask-api
    ```
2.  Start the development environment:
    ```bash
    docker-compose up --build
    ```
3.  The API will be available at `http://localhost:8000`.
4.  Run tests (in a new terminal):
    ```bash
    docker-compose exec web pytest
    ```

## 🔨 Usage

1.  **Create a User:** `POST /api/users/`
2.  **Get JWT Tokens:** `POST /api/token/`
3.  **Create a Workspace:** `POST /api/workspaces/` (Use the JWT token in the Authorization header)
4.  **Explore the real-time features:** Open multiple browser tabs on a board page and see updates live.

## 🤝 Contributing
(Outline how to contribute, though it's your project. It shows foresight.)

## 📝 License
This project is licensed under the MIT License.
