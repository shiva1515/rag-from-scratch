# Environment Setup

The notebooks may use different libraries, so dependencies are notebook-specific. Check the first cells of a notebook for its packages, models, and any external services before running it.

## Create a virtual environment

From the repository root:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install jupyterlab
```

On macOS or Linux, activate the environment with:

```bash
source .venv/bin/activate
```

## Start JupyterLab

```bash
jupyter lab
```

Open a notebook in one of the module folders listed in the main README. Install any additional packages specified by that notebook into the active environment.
