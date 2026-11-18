# MTH321 Project 3

Project 3 workspace for the MTH321 coursework. The repository follows the directory structure of [Project 2](https://github.com/brisssa113/MTH321-project-02).

## Current status

The repository contains the initial project structure. The topic, implementation, dependencies, numerical results and submission documents will be added as the project develops.

## Repository layout

```text
MTH321-project-03/
|-- README.md
|-- requirements.txt
|-- .gitignore
|-- code/
|   `-- tests/
|-- data/
|-- figures/
|-- generated/
|-- report/
`-- slides/
```

| Location | Purpose |
| --- | --- |
| `code/` | Numerical methods, experiment scripts and the eventual reproduction entry point |
| `code/tests/` | Automated checks for the implementation |
| `data/` | Numerical result tables, input data when needed, and run metadata |
| `figures/` | Figures used in the report and presentation |
| `generated/` | Generated table fragments, report values and other report-ready exports |
| `report/` | Report PDF and any report sources selected for submission |
| `slides/` | Presentation PDF and editable presentation sources |
| `requirements.txt` | Python dependencies, to be pinned when the implementation is chosen |

The `.gitkeep` files retain otherwise empty directories on GitHub and can be removed when real files are added. Keep the repository guide and dependency list at the repository root.

## Python environment

Once the required packages have been added to `requirements.txt`, run the following from the project root in PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

The experiment entry point and expected outputs will be documented here once implemented.

## Synchronising the local folder with GitHub

This is a Git repository. Local edits are uploaded with a commit and push; changes made on GitHub are downloaded with a pull.

Before editing, download any remote changes:

```powershell
cd D:\MTH321-project-03
git pull --ff-only
```

After editing, review and upload the intended files:

```powershell
git status
git add README.md requirements.txt .gitignore code data figures generated report slides
git diff --cached --stat
git commit -m "Describe the project update"
git push
```

## Submission checklist

- Document the chosen problem, methods and reproduction commands in this README.
- Pin the dependencies used for the submitted numerical results.
- Include the final code, numerical results, report and slides in their corresponding directories.
- Verify that the documented commands reproduce the reported numerical material.
- Record the appropriate source commit in the report after finalising the code and data.
