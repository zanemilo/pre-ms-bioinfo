Centralized repo for my prep work before the M.S. in Bioinformatics.  
Keep in mind the Pareto principle → 20% of effort for 80% of results.

Pillars, sub-tasks, and workflow subject to change.

---

## Setup — venv and Jupyter (how to start)

Recommended Python: 3.8+.

1. Create a virtual environment (from project root)
    - python -m venv .venv

2. Activate the venv
    - Windows (PowerShell): .venv\Scripts\Activate.ps1
    - Windows (cmd): .venv\Scripts\activate.bat
    - macOS / Linux: source .venv/bin/activate

3. (Optional) Upgrade pip and install dependencies
    - python -m pip install --upgrade pip setuptools
    - pip install -r requirements.txt
    - If you don't have a requirements file yet: pip install jupyter notebook numpy pandas scipy matplotlib seaborn

4. Start Jupyter Notebook
    - jupyter notebook
    - or: jupyter lab (if you prefer JupyterLab)

5. When finished
    - deactivate

Include a requirements.txt and a simple kernel install if you want the venv to appear in Jupyter's kernel list:
- python -m ipykernel install --user --name=myenv --display-name="Python (myenv)"

## Running examples and resuming work

- Run interactively
  - Start Jupyter (see above), open notebooks in examples/ or experiments/, and run cells.
  - To run a Python script: python path/to/script.py

- Run a notebook non-interactively (CI / quick run)
  - jupyter nbconvert --to notebook --execute path/to/notebook.ipynb --output executed.ipynb

- Quick checks
  - Run a small example: python examples/example_script.py (adjust path/name)

- Committing progress
  - git add <files>
  - git commit -m "brief note"
  - git push origin <branch>

- Resume work later
  1. cd /path/to/project
  2. Activate venv: .venv/Scripts/activate  (or platform equivalent)
  3. (If needed) pip install -r requirements.txt
  4. Start Jupyter: jupyter notebook (or jupyter lab) and open your notebook
  5. If the venv kernel is not listed, reinstall the kernel:
     - python -m ipykernel install --user --name=myenv --display-name="Python (myenv)"
  6. Pull updates if collaborating: git pull

- Cleanup when done
  - deactivate
  - remove temporary files or checkpoints as needed

This makes it easy to run examples, save work, and come back to the project later.

---

## Main Pillars to tackle

### 1. Stats 
- Descriptive stats 
- Key distributions (Normal, Binomial, Poisson)
- Hypothesis testing (t-test, chi-square)
- Correlation & regression
- Multiple testing correction (FDR)

### 2. Biology
- Cell/molecular basics
- Genetics & genomics
- Microbiology fundamentals

### 3. Programming
- Python (`numpy`, `pandas`, `scipy`, `matplotlib`, `seaborn`)
- R (`tidyverse`, `ggplot2`, `stats`)
- Reusable notebook templates

---

## Workflow
- **Learn** → skim core concept  
- **Code** → small example in `examples/`  
- **Apply** → mini experiment in `experiments/`  

---

## Current Focus
- [x] Visualization example notebook (Matplotlib) -> Plans to expand further libs 
- [x] Distributions example notebook
- [x] Iris dataset example notebook (Pandas/Seaborn)
- [ ] Regression example notebook
- [ ] Correlation example notebook
- [ ] Multiple testing correction (FDR) example notebook
- [ ] ML example notebook -> as it pertains to bioinformatics
- [ ] Apply Hypothesis testing to a dataset

## TO DO
- [x] Venv
- [x] Jupyter setup
- [x] Other dependencies
- [x] GitHub repo
- [x] Hypothesis testing Jupyter example notebook 
- [ ] R setup and example notebook
- [ ] Add further objectives to README
