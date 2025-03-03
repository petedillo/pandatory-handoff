# Pandatory Handoff Packet

**Project Name:** Pandatory

**Prepared By:** Pedro Delgadillo

## 1. Introduction

This document serves as a handoff packet for the Pandatory project, a web application designed for efficient pantry management. It provides essential information for future developers and maintainers.

## 2. Project Overview

Pandatory is built using modern web technologies, offering a user-friendly experience for organizing pantry needs.

## 3. Key Links

* **Figma Design:** [Figma](https://www.figma.com/proto/O4NyxyuY00i7yA3y5uR5xD/Pandatory?node-id=0-1&t=qdDw0GWlaujflfIK-1)
* **GitHub Repository:** [https://github.com/petedillo/pandatory](https://github.com/petedillo/pandatory)
* **Deployed Frontend:** [https://pandatory.vercel.app/](https://pandatory.vercel.app/)

## 4. System Architecture

Pandatory utilizes a Dockerized architecture, comprising the following components:

* **Frontend:** React/Vite application.
* **Backend:** Express/Node.js API.
* **Database:** PostgreSQL.

## 5. Port Information

The application utilizes the following ports:

* **Frontend:** `5173` (accessible at `http://localhost:5173`)
* **Backend API:** `3000` (accessible at `http://localhost:3000`)
* **PostgreSQL Database:** `5432` (accessible at `http://localhost:5432` - primarily for internal Docker communication)

## 6. Development Environment Setup

### 6.1 Prerequisites

* Docker: [Install Docker](https://www.docker.com/)
* Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/)

### 6.2 Running the Application

1.  **Clone the Repository:**

    ```bash
    git clone [https://github.com/petedillo/pandatory](https://github.com/petedillo/pandatory)
    cd pandatory
    ```

2.  **Start the Application:**

    ```bash
    docker compose up
    ```

3.  **Run Database Migrations:**

    ```bash
    docker compose exec backend npm run migrate
    ```

4.  **Seed the Database (Optional):**

    ```bash
    docker compose exec backend npm run seed
    ```

5.  **Access the Application:**

    * Frontend: [http://localhost:5173](http://localhost:5173)
    * Backend API: [http://localhost:3000](http://localhost:3000)

6.  **Stopping the Application:**

    ```bash
    docker-compose down
    ```

## 7. Database Information

* Database: PostgreSQL
* Port: 5432
* Migrations and seed data are located in the backend folder.

## 8. Backend API Documentation

* [API Endpoints Documentation](ENDPOINTS.md)

## 9. Frontend Information

* The frontend is built with React and Vite.
* Relevant components and state management are located within the `src` directory.
* Styling information is located in the `src/assets/styles` directory.

## 10. Future Considerations

* Implementing a barcode scanner for easier inventory management.

## 11. Contact Information

* Pedro Delgadillo
* pedelgadillo@gmail.com
* PeteDillo