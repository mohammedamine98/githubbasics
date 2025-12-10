# Lab 1: GitHub Basics - Version Control and Automated Testing

## Learning Objectives

- Use Git for version control
- Write and run unit tests (pytest and unittest)
- Set up GitHub Actions for automated testing

## Prerequisites

- Python 3.8+
- Git installed
- GitHub account

## Setup Instructions

### 1. Clone the Repository

**Mac:**
```bash
git clone https://github.com/AardwolfFizzler/MLOPS.git
cd MLOPS-Repo/labs/lab1-github-basics
```

**Windows:**
```bash
git clone https://github.com/AardwolfFizzler/MLOPS.git
cd MLOPS-Repo\labs\lab1-github-basics
```

### 2. Create Virtual Environment

**Mac:**
```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## Project Structure

```
lab1-github-basics/
├── .github/workflows/     # GitHub Actions
├── src/
│   ├── __init__.py
│   └── calculator.py      # Main code
├── test/
│   ├── __init__.py
│   ├── test_pytest.py
│   └── test_unittest.py
├── requirements.txt
└── README.md
```

## Running Tests Locally

**Pytest (Mac):**
```bash
pytest test/test_pytest.py -v
```

**Pytest (Windows):**
```bash
pytest test\test_pytest.py -v
```

**Unittest (Mac):**
```bash
python -m unittest test.test_unittest -v
```

**Unittest (Windows):**
```bash
python -m unittest test.test_unittest -v
```

## Git Workflow

```bash
# Check status
git status

# Add changes
git add .

# Commit
git commit -m "Your message"

# Push to GitHub
git push origin main

# Create new branch
git checkout -b feature/your-feature
```

## Lab Tasks

1. **Setup**: Clone repo, create virtual environment, install dependencies
2. **Run Tests**: Run both pytest and unittest locally
3. **Make Changes**: Create a new branch, add a division function `fun5(x, y)`
4. **Write Tests**: Add tests for your new function
5. **Push & PR**: Push changes and create a Pull Request
6. **GitHub Actions**: Verify automated tests pass

## Troubleshooting

**Virtual environment won't activate (Windows):**
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

**Tests fail:**
- Verify Python version: `python --version`
- Reinstall dependencies: `pip install -r requirements.txt`

## Resources

- [Git Documentation](https://git-scm.com/doc)
- [Pytest Docs](https://docs.pytest.org/)
- [GitHub Actions](https://docs.github.com/en/actions)

---

**Happy Coding**