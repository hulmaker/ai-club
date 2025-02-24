The goal is to analyze the data containing records of swimming pool occupancy.


The data are stored in `logs/sutka.csv` with columns:

 - timestamp: Timestamp of the reading with the following format `YYYY-MM-DD HH:MM:SS`
 - percentage: The occupancy percentage
 - pool: Number swimming pool visitors
 - aquapark: Number of aquapark visitors


Dev environment setup:

 - Use `uv` package manager available from `/opt/homebrew/bin/uv` to create a new python 3.13 project.
 - Use the following packages: `pandas, numpy, pyplot, pytest, seaborn`
 - Save the project state in `pyproject.toml` file.
 - Set reasonably strict linting and formatting rules for the `ruff` formatter.


To finish the project, we need to do the following steps:

1. Load the data from the csv file.
2. Make sure the loading is correct by writing unit tests. Check the number of lines is correct.
3. Analyze the data: do not create jupyter notebooks, only python scripts. Do not save the plot as an image, running the file opens a new pyplot window with the following plots:
    - A line plot to compare the occupancy by week day
    - A heatmap to compare the number of pool visitors on hourly basis. Categorized by a week day.


---

# Prompts

Create a new project with python 3.13 and `uv` package manager available from `/opt/homebrew/bin/uv`. Create a project as described in @general-python.mdc 

Outline the project structure, create folders and unit tests. Fix any bugs until all unit tests pass.


---

 - Load the data from the csv file as described in the @general-python.mdc. Implement unit tests and iterate untill all the tests pass without errors.
 - Format the code with `uv tool run ruff format`
 - Use linter with `uv tool run ruff check --fix` and fix any remaining problems.


---

Let's plot the data and see the results.

Use the TODO function to load read the data.
Then make plots described in the @general-python.mdc
Make sure the legend and all axes are described.
Make sure the code works and does not fail with an error.