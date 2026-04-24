# KAIM - Week 0: Climate Change Challenge

## Project Overview
This project is part of the 10 Academy (KAIM) Intensive Training. Week 0 focuses on establishing a professional engineering foundation. This includes setting up a reproducible development environment, implementing version control best practices, and establishing a Continuous Integration (CI) pipeline.

## Objectives
- **Version Control**: Utilize Git for branching, committing (Conventional Commits), and merging via Pull Requests.
- **Environment Management**: Setup Python virtual environments for dependency isolation.
- **CI/CD**: Automate dependency installation and environment verification using GitHub Actions.
- **Project Structure**: Organize the repository for scalability in data science and engineering tasks.

## Project Structure
The repository follows a modular structure to separate concerns:
- `.github/workflows/`: Contains the CI (`ci.yml`) configurations.
- `notebooks/`: Jupyter notebooks for data exploration and visualization.
- `scripts/`: Modular Python scripts for reusable logic.
- `src/`: Core source code for the project.
- `tests/`: Unit tests to ensure code quality.

## Setup Instructions

### Prerequisites
- Python 3.8+
- Git

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/b-ezawit/climate-challenge-week0.git
   cd climate-challenge-week0
   ```

2. **Set up Virtual Environment:**
   ```bash
   python -m venv .venv
   # Activate on Windows:
   .\.venv\Scripts\activate
   # Activate on Mac/Linux:
   source .venv/bin/activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Continuous Integration
A GitHub Actions workflow is configured to run on every push to the `main` branch. It ensures that the environment can be built successfully by installing all listed dependencies in `requirements.txt`.

EOF# Ensure you are on the setup-task branch
git checkout setup-task

# Create the detailed KAIM content
cat <<EOF > README.md
# KAIM - Week 0: Climate Change Challenge

## Project Overview
This project is part of the 10 Academy (KAIM) Intensive Training. Week 0 focuses on establishing a professional engineering foundation. This includes setting up a reproducible development environment, implementing version control best practices, and establishing a Continuous Integration (CI) pipeline.

## Objectives
- **Version Control**: Utilize Git for branching, committing (Conventional Commits), and merging via Pull Requests.
- **Environment Management**: Setup Python virtual environments for dependency isolation.
- **CI/CD**: Automate dependency installation and environment verification using GitHub Actions.
- **Project Structure**: Organize the repository for scalability in data science and engineering tasks.

## Project Structure
The repository follows a modular structure to separate concerns:
- `.github/workflows/`: Contains the CI (`ci.yml`) configurations.
- `notebooks/`: Jupyter notebooks for data exploration and visualization.
- `scripts/`: Modular Python scripts for reusable logic.
- `src/`: Core source code for the project.
- `tests/`: Unit tests to ensure code quality.

## Setup Instructions

### Prerequisites
- Python 3.8+
- Git

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/b-ezawit/climate-challenge-week0.git
   cd climate-challenge-week0
   ```

2. **Set up Virtual Environment:**
   ```bash
   python -m venv .venv
   # Activate on Windows:
   .\.venv\Scripts\activate
   # Activate on Mac/Linux:
   source .venv/bin/activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Continuous Integration
A GitHub Actions workflow is configured to run on every push to the `main` branch. It ensures that the environment can be built successfully by installing all listed dependencies in `requirements.txt`.

