# DevOps CI Experiment Using GitHub Actions

This project demonstrates how to set up **Continuous Integration (CI)** for a simple Python project using **GitHub Actions**. The workflow automatically runs tests whenever code is pushed or a pull request is created.

---

## 📌 Steps to Reproduce

### 1. Create Project Locally
```bash
mkdir devops-demo
cd devops-demo
```

### 2. Create Required Files
```bash
touch main.py test_main.py
mkdir -p .github/workflows
touch .github/workflows/python-app.yml
```

### 3. Initialize Git and Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit - Python project with GitHub Actions CI"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

---

## 📝 Project Structure
```
devops-demo/
│
├── main.py                  # Simple Python program
├── test_main.py             # Unit tests for main.py
│
└── .github/
    └── workflows/
        └── python-app.yml   # GitHub Actions CI workflow configuration
```

---
## ✅ Running the CI

1. Push the code to your GitHub repository.
2. Go to the **Actions** tab in your GitHub repo.
3. The workflow will automatically trigger and show the test results.

## 🚀 Outcome

- Every time you **push** or create a **pull request**, GitHub Actions will:
  - Checkout the code
  - Set up Python
  - Install dependencies
  - Run all tests using `pytest`

You can view the workflow status under the **Actions** tab.
