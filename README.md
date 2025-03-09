# How to Install SQLMap on Ubuntu Using a Virtual Environment

This guide will walk you through installing SQLMap on Ubuntu using a Python virtual environment. A virtual environment is an isolated Python environment where you can install packages without affecting the system-wide Python installation.

## Step 1: Install python3-venv
If not already installed, install the python3-venv package to create virtual environments.

```bash
sudo apt install python3-venv
```

## Step 2: Create a Virtual Environment
Create a virtual environment named `sqlmap-env` (or any name you prefer).

```bash
python3 -m venv sqlmap-env
```

## Step 3: Activate the Virtual Environment
Activate the virtual environment to isolate your Python environment.

```bash
source sqlmap-env/bin/activate
```

Once activated, your terminal prompt will change to indicate the virtual environment is active.

## Step 4: Install SQLMap Using pip
Install SQLMap using pip inside the virtual environment.

```bash
pip install sqlmap
```

## Step 5: Verify the Installation
Check if SQLMap is installed correctly by running:

```bash
sqlmap --version
```

## Step 6: Deactivate the Virtual Environment
When you're done using SQLMap, deactivate the virtual environment to return to the system-wide Python environment.

```bash
deactivate
```

## Summary of Commands
Here’s a quick summary of all the commands:

```bash
# Install python3-venv
sudo apt install python3-venv

# Create a virtual environment
python3 -m venv sqlmap-env

# Activate the virtual environment
source sqlmap-env/bin/activate

# Install SQLMap
pip install sqlmap

# Verify installation
sqlmap --version

# Deactivate the virtual environment
deactivate
```

## Notes
- Using a virtual environment ensures that SQLMap and its dependencies are isolated from the system-wide Python installation.
- Always ensure you have permission to test the target website. **Unauthorized testing is illegal.**

