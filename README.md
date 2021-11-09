# ptsa

The package "**p**eriodic **T**-matrix **s**cattering **a**lgorithms" provides a
framework to simplify computations of the electromagnetic scattering of waves at finite
and periodically infinite arrangements of particles. All methods are suitable for the
use of chiral materials.

## Installation

### Installation using pip

To install the package with pip, use

```sh
pip install git+https://git.scc.kit.edu/photonics/ptsa.git
```

### Installation for development

1. Clone the repository with

```sh
git clone git@git.scc.kit.edu/photonics/ptsa.git
```

or

```sh
git clone https://git.scc.kit.edu/photonics/ptsa.git
```

and enter the directory
```sh
cd ptsa
```

2. Create a conda environment with

```sh
conda env create -f environment.yml
```

which installs all packages needed for building and running ptsa, testing, different
benchmarks, and building the documentation. Activate the environment:

```sh
conda activate ptsa-dev
```

3. Setup the package with

```sh
python setup.py develop
```

4. And finally install the current directory with conda

```sh
conda develop .
```

This last step makes the program available in the environment independently of the
current folder. This is especially necessary for correctly building the documentation.

## Documentation
The code is documented with docstrings and `sphinx`. Go into `docs` and run `make html`
and you'll find a nice HTML-page at `docs/_build/index.html`. For this to work properly,
install it using the development environment method.

## Features

* [x] T-matrices using a spherical and using a cylindrical basis set
* [x] Calculations in helicity basis, enabling the use of chiral media throughout
* [x] Scattering from clusters of particles
* [x] Scattering from particles and clusters arranged in 3d-, 2d-, and 1d-lattices
* [x] Calculation of light propagation in stratified media
* [x] Band calculation in crystal structures
