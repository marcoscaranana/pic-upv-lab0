# Lab0.1 & Lab0.2 Modesolver: Waveguides & Couplers

This repository contains notebooks to validate that the core dependencies for Lab0.1 and Lab0.2 are installed and working. The intended workflow is VS Code on Windows with a WSL (Linux) environment.

## Prerequisites (Windows + WSL)

- Windows 10/11 with WSL 2 enabled.
- A Linux distribution installed via WSL (e.g., Ubuntu 22.04).
- VS Code with the **WSL** extension installed.
- Python 3.10+ available inside WSL.

If you have not configured WSL yet, follow the official Microsoft setup guide and then open VS Code connected to WSL.

## Open the project in WSL

1. Open a WSL terminal.
2. Navigate to the repo folder (or clone it):
   - Fork the repository on GitHub.
   - Clone your fork: `git clone <your-fork-url>`
   - Then: `cd pic-upv-lab0`

VS Code will reopen the folder using the WSL remote environment.

## Create and select a Python environment

From the VS Code WSL window:

1. Ensure **uv** is installed in WSL.
2. Sync the dependencies from `pyproject.toml`:
   - `uv sync`
3. Select the interpreter in VS Code:
   - Command Palette → **Python: Select Interpreter** → choose the `.venv` created by uv (if prompted).

## Install dependencies

Use the repo’s `pyproject.toml` via uv:

```bash
uv sync
```

## Run the notebooks

1. Open a notebook from the Notebooks folder in VS Code:
   - [NoteBooks/010_MODESOLVER_Student.ipynb](NoteBooks/010_MODESOLVER_Student.ipynb)
   - [NoteBooks/020_COUPLERS_v2025_Student.ipynb](NoteBooks/020_COUPLERS_v2025_Student.ipynb)
2. Select the kernel named **pic-upv-lab0**.
3. Run the cells top-to-bottom.

You should see the expected plots in the output cells.

## Troubleshooting

- Email: cccanvas@upv.es