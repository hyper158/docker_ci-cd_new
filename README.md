# CI/CD Pipeline using GitHub Actions and Docker

## 📌 Experiment No. 6

### Title

Configuration of a CI/CD workflow to automatically build, test, and publish Docker images using GitHub Actions.

---

## 🎯 Objective

To design and implement a Continuous Integration and Continuous Deployment (CI/CD) workflow that automates the process of building, testing, and containerizing a FastAPI application.

---

## 📖 Overview

This project demonstrates the basic implementation of a CI/CD pipeline using GitHub Actions integrated with Docker. The workflow is triggered whenever code changes are pushed to the repository. It ensures that the application is automatically tested, built into a Docker image, and prepared for deployment.

The aim is to understand how automation improves efficiency, reduces manual effort, and ensures consistency in software delivery.

---

## 🛠️ Technologies Used

* Python (FastAPI)
* Docker
* GitHub Actions
* Pytest

---

## 📂 Project Structure

```id="1j4qgy"
ci-cd-fastapi/
│
├── Dockerfile
├── requirements.txt
├── app/
│   ├── main.py
│   └── test_main.py
└── .github/
    └── workflows/
        └── ci-cd.yml
```

---

## ⚙️ Workflow Summary

The CI/CD pipeline performs the following steps:

1. Retrieves the latest code from the repository
2. Installs required dependencies
3. Executes test cases to validate functionality
4. Builds a Docker image of the application
5. Prepares the image for deployment to a container registry

---

## 🚀 Local Execution

To run the application locally using Docker:

1. Build the Docker image:

```id="cjg8r1"
docker build -t fastapi-app .
```

2. Run the container:

```id="0ljqdt"
docker run -p 8000:8000 fastapi-app
```

3. Access the application:

```id="x3zthc"
http://localhost:8000
```

---

## 📊 Expected Output

The application returns a simple JSON response:

```id="7bkavf"
{"message": "Hello CI/CD World"}
```

---

## ✅ Conclusion

This experiment demonstrates the fundamentals of CI/CD automation using GitHub Actions and Docker. It highlights how automated workflows can streamline the process of integration, testing, and deployment, making software development more efficient and reliable.

---
