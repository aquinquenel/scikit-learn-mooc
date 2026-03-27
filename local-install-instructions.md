# Local install instructions

The course uses Python 3 and some data analysis packages such as Numpy, Pandas,
scikit-learn, and matplotlib.

## Install UV

**This step is only necessary if you don't have UV installed already**:

- follow the installation instructions [here](https://docs.astral.sh/uv/getting-started/installation/)

## Set up the project

```sh
# Clone this repo
git clone https://github.com/INRIA/scikit-learn-mooc
cd scikit-learn-mooc
# Install the dependencies with UV:
uv sync
```

## Check your install

To make sure you have all the necessary packages installed, we **strongly
recommend** you to execute the `check_env.py` script located at the root of
this repository:

```sh
uv run python check_env.py
```

Make sure that there is no `FAIL` in the output when running the `check_env.py`
script, i.e. that its output looks similar to this:

```
[ OK ] numpy version 1.19.5
[ OK ] scipy version 1.6.0
[ OK ] matplotlib version 3.3.3
[ OK ] sklearn version 1.6
[ OK ] pandas version 2.0
[ OK ] seaborn version 0.13
[ OK ] notebook version 6.2.0
[ OK ] plotly version 5.10.0
```

## Run Jupyter notebooks locally

```sh
uv run jupyter notebook full-index.ipynb
```

`full-index.ipynb` is an index file helping to navigate the notebooks.
All the Jupyter notebooks are located in the `notebooks` folder.
