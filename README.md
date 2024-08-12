 # Lab image interpretation

To get started, clone the repo, create a new virtual environment and install the dependencies using the following commands:

```bash
git clone https://github.com/florisdf/labo_bld_interp.git
cd labo_bld_interp
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Then start Jupyter Lab by running (still from inside the `labo_bld_interp` repo folder):

```bash
jupyter lab
```

This command should open Jupyter Lab in your web browser. In the file explorer of Jupyter Lab, click on `notebooks` and open `01_inspect_data.ipynb`.

## I want all solutions

A reference solution is stored for each notebook in hidden patch files. To obtain these solutions, create a copy of your own version of the notebook, checkout the notebook from Git and run the `utils/clear_code_cells.py` script. For example, for the notebook `01_inspect_data.ipynb`, you can do this by running the following commands from inside the `labo_bld_interp` repo directory:

```bash
cp notebooks/01_inspect_data.ipynb notebooks/01_inspect_data_MY_SOLUTION.ipynb
git checkout notebooks/01_inspect_data.ipynb
python utils/clear_code_cells.py --undo notebooks/01_inspect_data.ipynb
```

Now, `notebooks/01_inspect_data.ipynb` will contain the reference solution.
