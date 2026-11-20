# SQL Learning

SQL practice covering filtering, sorting, grouping, joins, and common table expressions.

- `sql_lesson_1_essentials.ipynb` — Lesson 1 notebook.
- `lesson1.db` — SQLite database with 12 experiments and 12 matching samples. All values are synthetic.
- `environment.yml` — Conda dependencies.

## Setup

Run these commands in the Ubuntu WSL terminal. This project uses Conda.

```bash
cd ~/projects/sql-learning
conda activate sql-learning
```

For a new environment, create it first:

```bash
conda env create -f environment.yml
conda activate sql-learning
```

To update an existing environment's dependencies:

```bash
conda env update -f environment.yml
```

`environment.yml` lists Python 3.12, the notebook kernel, JupyterLab, and pandas for table display. SQLite is included with Python.

## Use

Open this folder in VS Code through WSL, with the Python and Jupyter extensions installed. Open `sql_lesson_1_essentials.ipynb` and select the `sql-learning` Conda environment as its kernel. Run the connection cell first, then the query cells.

Alternatively, run `jupyter lab` from the activated environment.

Keep the notebook and `lesson1.db` together and launch from this folder. The database is ready to use; no SQL setup scripts or database server are needed.

Run `conda deactivate` when finished.

## References

- [SQLBolt](https://sqlbolt.com/)
- [Data With Danny — PostgreSQL for Data Analytics](https://github.com/datawithdanny/postgresql-for-data-analytics)
