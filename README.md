# MessyStash-Documentaion

mkdocs wiki style documentation for MessyStash school project

## 1. Prerequisites

- Git
- Python 3.10+
- Pip

### Linux - Debian-based

Install the required packages:

```bash
sudo apt update
sudo apt install -y git python3 python3-venv python3-pip
```

Verify installation:

```bash
git --version
python3 --version
```

### Windows

Install the prerequisites using each of their official methods

> _You have google you can figure it out_

## 2. Clone the repo

```bash
git clone https://github.com/Kkiriya/MessyStash-Documentaion.git
cd MessyStash-Documentation
```

## 3. Create and activate a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

You should now see (.venv) at the beginning of your terminal prompt

## 4. Install dependencies

With the virtual environment activated:

```bash
python -m pip install -r requirements.txt
```

This installs the versions of MkDocs, Material for MkDocs, and any plugins defined in your repository's requirements.txt.

## 5. Start the local documentation server

```bash
mkdocs serve
```

Open http://127.0.0.1:8000/ in your browser.

MkDocs automatically reloads when Markdown or configuration files change.

## 6. Stop the server

Press `Ctrl+C` to stop the server, then deactivate the virtual environment:

```bash
deactivate
```

## 7. Next time you work on the repo

```bash
cd MessyStash-Documentation
git pull
source .venv/bin/activate
mkdocs serve
```
