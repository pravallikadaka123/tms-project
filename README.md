### 📌 Task Management System (TMS)
A full-stack web application that enables users to create, update, view, and delete tasks efficiently. Built with **Java (Spring Boot)** on the backend, **Angular** on the frontend, **Oracle SQL** for the database, and deployed on **AWS**.

### 🚀 Features

🔹 User-friendly interface to manage tasks

🔹 Create, view, update, and delete tasks (CRUD)

🔹 Responsive Angular frontend

🔹 RESTful API built with Spring Boot (or Go)

🔹 Oracle SQL integration for data storage

🔹 AWS deployment with EC2 (backend), RDS (database), and S3 (optional for frontend)

🔹 (Optional) JWT authentication and role-based access control

🔹 (Optional) CI/CD pipeline using GitHub Actions or AWS CodePipeline


### 🛠️ Tech Stack

| Layer      | Technology                            |
| ---------- | ------------------------------------- |
| Frontend   | Angular                               |
| Backend    | Java (Spring Boot)                    |
| Database   | Oracle SQL                            |
| Deployment | AWS (EC2, RDS, S3, Elastic Beanstalk) |
| CI/CD      | GitHub Actions / AWS CodePipeline     |

### 📦 Architecture

[Angular Frontend]  <--->  [Java Spring Boot Backend]  <--->  [Oracle SQL Database (RDS)]
                                 |
                                 V
                              [AWS EC2/S3]



🗂️ Project Structure
bash
Copy
Edit
tms-project/
│
├── backend/               # Spring Boot backend
│   ├── src/main/java/...  # Controllers, Services, Models
│   ├── src/main/resources
│   └── pom.xml
│
├── frontend/              # Angular frontend
│   ├── src/app/...
│   └── angular.json
│
├── infra/                 # AWS deployment & CI/CD
│   ├── aws/
│   └── cicd/
│
├── docs/                  # Documentation
│
├── .gitignore
└── README.md
🖥️ Getting Started
🔧 Prerequisites
Java 17+ or Go (if you choose Go)

Node.js + Angular CLI

Oracle SQL (local or AWS RDS)

AWS account

🔨 Backend Setup
bash
Copy
Edit
cd backend
# For Maven
mvn clean install
mvn spring-boot:run

# For Gradle (if applicable)
gradle bootRun
🔨 Frontend Setup
bash
Copy
Edit
cd frontend
npm install
ng serve --open
🔨 Database Setup
Import schema.sql in Oracle SQL (locally or AWS RDS).

Configure DB credentials in application.properties.

🔨 AWS Deployment
Backend: Deploy using EC2 or Elastic Beanstalk.

Database: Use Oracle RDS for scalable database hosting.

Frontend: Host Angular app on S3 or deploy via Elastic Beanstalk.

(Optional) Set up CI/CD using GitHub Actions or AWS CodePipeline.

✨ Contributing
Fork the repository

Create a new branch (git checkout -b feature/awesome-feature)

Commit your changes (git commit -m 'Add awesome feature')

Push to the branch (git push origin feature/awesome-feature)

Open a Pull Request

📄 License
This project is licensed under the MIT License.

🙌 Acknowledgments
Spring Boot team

Angular team

AWS free tier for testing deployments
