# CI/CD Pipeline using GitHub Actions and Docker

This project demonstrates how to create a basic **CI/CD pipeline** using **GitHub Actions**. The pipeline automatically builds, tests, and deploys a Node.js application using Docker.

 🚀 What It Does

Whenever you push code to the `main` branch:
1. The latest code is pulled from the GitHub repository.
2. Node.js is installed on a virtual machine.
3. Dependencies are installed using `npm install`.
4. Tests are run using `npm test`.
5. A Docker image is built from the app.
6. The Docker image is pushed to DockerHub.



 🔧 Technologies Used

- **GitHub Actions** – for automation
- **Node.js** – backend platform
- **Docker** – to containerize the application
- **DockerHub** – to store the Docker image
- **GitHub Secrets** – to securely store DockerHub username and password



 📁 Files Included

- `.github/workflows/ci-cd.yml` – The GitHub Actions pipeline file
- `Dockerfile` – Defines how the Docker image is built
- `package.json` – Node.js project metadata and dependencies
- `README.md` – This file
- (Add any screenshots here if you have)



 🔐 GitHub Secrets Required

Before using this workflow, add the following secrets to your GitHub repository:

- `USERNAME` – your DockerHub username
- `PASSWORD` – your DockerHub password or access token



 
 📦 How to Use

1. Clone the repository.
2. Set up your project with a `Dockerfile` and `package.json`.
3. Push the code to GitHub.
4. Make sure you push to the `main` branch.
5. The workflow will run automatically and push the Docker image to your DockerHub account.



 📝 Notes

- Make sure the DockerHub repo name and tag match in the workflow file.
- You can extend this pipeline to deploy to cloud platforms like Render, AWS, or Heroku.



 ✅ Output

After the pipeline runs:
- Your app is containerized into a Docker image.
- The image is available in your DockerHub account.

