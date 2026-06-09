# ProgrammongForDA
# ProgrammongForDA

A Python-based project for Data Analytics using modern Python tooling with **uv**, **Pandas**, and **Jupyter Notebook**.

## Project Setup

### Prerequisites

* Python 3.12.1
* pip 26.1.2
* uv 0.11.19

Verify your Python installation:

```bash
python --version
```

Output:

```text
Python 3.12.1
```

---

## Installation

### 1. Install uv

```bash
pip install uv
```

### 2. Upgrade pip

```bash
python3 -m pip install --upgrade pip
```

### 3. Initialize the Project

```bash
uv init
```

This creates the project configuration files and initializes the Python project.

---

## Virtual Environment

A virtual environment was created using uv:

```bash
uv venv --python 3.11 --seed
```

> Note: The project requires Python 3.12 or higher. When dependencies were added, uv automatically recreated the environment using Python 3.12.1.

Activate the environment:

```bash
source .venv/bin/activate
```

---

## Dependencies

### Data Analysis Library

Install Pandas:

```bash
uv add pandas
```

Installed packages:

* pandas 3.0.3
* numpy 2.4.6
* python-dateutil 2.9.0
* six 1.17.0

### Jupyter Environment

Install Jupyter Notebook and IPython Kernel:

```bash
uv add jupyter ipykernel
```

This installs:

* Jupyter Notebook
* JupyterLab
* IPython
* ipykernel
* Widgets support
* Notebook conversion tools
* Additional Jupyter ecosystem packages

---

## Project Structure

```text
ProgrammongForDA/
│
├── .venv/
├── app/
│   └── FileHandeling.ipynb
│
├── data/
│
├── FileHandeling.ipynb
│
├── pyproject.toml
├── uv.lock
└── README.md
```

### Directory Description

| Directory/File        | Purpose                                                  |
| --------------------- | -------------------------------------------------------- |
| `data/`               | Store datasets and raw data files                        |
| `app/`                | Application notebooks and scripts                        |
| `FileHandeling.ipynb` | Notebook for file handling exercises and examples        |
| `pyproject.toml`      | Project configuration and dependencies                   |
| `uv.lock`             | Locked dependency versions for reproducible environments |

---

## Running the Project

Activate the virtual environment:

```bash
source .venv/bin/activate
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Or launch JupyterLab:

```bash
jupyter lab
```

---

## Technologies Used

* Python 3.12.1
* uv
* Pandas
* NumPy
* Jupyter Notebook
* JupyterLab
* IPython Kernel

---

## Learning Objectives

This repository is intended for practicing and developing skills in:

* Data Analysis
* Data Manipulation with Pandas
* File Handling in Python
* Jupyter Notebook Workflows
* Python Virtual Environment Management
* Dependency Management with uv

---

## Author

**Ali Vaisifard**

Data Analytics Learning Project
