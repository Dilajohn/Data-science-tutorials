# Data Science Tutorials

This repository is a hands-on data science learning journey. Instead of trying to learn every concept in isolation, each topic is practiced through a small, concrete project. As the fundamentals become more familiar, the projects will grow in size and complexity, gradually introducing more realistic data, stronger analysis techniques, and more advanced tools.

The goal is to build practical understanding through repetition:

1. Learn a concept.
2. Apply it to a small dataset or project.
3. Inspect the result and fix mistakes.
4. Extend the project with a more advanced technique.
5. Keep the working code and lessons as a personal reference.

## Current Project

### Tabular data foundations

[`tabular_data.ipynb`](tabular_data.ipynb) uses a small real-estate dataset inspired by property listings in Mexico. The notebook currently practices:

- Python lists and nested lists
- Python dictionaries and lists of dictionaries
- Accessing values by position and by key
- `for` loops for row-wise calculations
- Calculating price per square meter
- Collecting values into a list for a column-wise calculation
- Calculating the mean house price
- Checking object types, lengths, and values while learning

The notebook deliberately starts with basic Python data structures. This makes the underlying data operations visible before introducing higher-level tools such as pandas.

## Learning Approach

This project follows a progressive, hands-on system:

### Stage 1: Core Python

- Variables and data types
- Lists, dictionaries, and nested structures
- Loops and conditional logic
- Functions and reusable calculations
- Reading errors and debugging code

### Stage 2: Working with tabular data

- Importing CSV files
- Loading data with pandas
- Selecting rows and columns
- Filtering and sorting observations
- Handling missing and inconsistent values
- Creating derived columns

### Stage 3: Exploratory data analysis

- Summary statistics
- Distributions and outliers
- Grouped comparisons
- Correlation and relationships between variables
- Clear data visualizations with matplotlib or seaborn

### Stage 4: Statistical reasoning

- Asking measurable questions
- Choosing useful comparisons
- Interpreting averages and variation
- Avoiding misleading conclusions
- Communicating findings with evidence

### Stage 5: Machine learning

- Preparing features and targets
- Splitting data into training and test sets
- Building baseline models
- Evaluating regression and classification models
- Comparing models and identifying limitations

### Stage 6: More advanced projects

- Larger and messier datasets
- Reusable Python modules
- Data pipelines
- Feature engineering
- Model interpretation
- Experiment tracking
- Deployment or interactive reporting

The exact order may change as new projects reveal which concepts need more practice.

## Getting Started

### Requirements

- Python 3.10 or newer
- Visual Studio Code
- The VS Code Python extension
- The VS Code Jupyter extension

The repository also contains a local `.venv` environment. If it is not available on another machine, create a new environment instead of committing environment files:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install jupyter
```

Open the repository folder in VS Code, open [`tabular_data.ipynb`](tabular_data.ipynb), select the Python kernel, and run the notebook cells from top to bottom.

## Recommended Notebook Workflow

1. Read the task description before running the cell.
2. Predict what the code should produce.
3. Run the cell and inspect the output.
4. Compare the result with the prediction.
5. Change one small part at a time when experimenting.
6. Restart the kernel and run all cells when execution order becomes confusing.
7. Add a short note when a mistake teaches an important lesson.

Notebook output is useful while learning, but the code should remain understandable when outputs are cleared and the notebook is run again from a fresh kernel.

## Project Standards

As the repository grows, each project should aim to include:

- A clear problem statement
- A description of the data
- Reproducible setup instructions
- Small, understandable steps
- Checks for assumptions and data quality
- Visual or numerical evidence for conclusions
- A short summary of what was learned
- Known limitations and possible next steps

The project should become more advanced over time without losing the central learning principle: understand the operation first, then use abstractions that make the operation faster and more reliable.

## Repository Structure

```text
.
|-- README.md
|-- tabular_data.ipynb
|-- .venv/                 # Local environment; do not commit its contents
```

Future projects can be organized into separate folders, for example:

```text
projects/
|-- 01-tabular-data/
|-- 02-data-cleaning/
|-- 03-exploratory-analysis/
|-- 04-predictive-modeling/
```

## Version Control Workflow

Save meaningful milestones as small commits. A useful commit message describes the learning change, for example:

```text
Add calculation of mean house price
Introduce pandas data cleaning workflow
Compare house prices by location
```

Before pushing a change:

```powershell
git status
git diff
git add .
git commit -m "Describe the learning milestone"
git push origin main
```

## Long-Term Goal

This repository is intended to show progress, not just finished answers. Early projects should make the fundamentals visible. Later projects should solve more realistic problems while preserving that same habit of asking:

- What question am I trying to answer?
- What does each value represent?
- What assumptions am I making?
- How can I check that the result is reasonable?
- What would make this analysis more reliable?

By building upward through increasingly complex projects, the aim is to develop both technical skill and the judgment needed to use data science responsibly.

## License

No license has been selected for this learning repository yet.