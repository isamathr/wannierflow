<h1 align="center"> wannierflow</h1>

Creator of the repository: Ilias Samathrakis

<p align="center">
  <img src="https://github.com/isamathr/wannierflow/assets/134223309/8243bc39-340d-42f6-9471-1d32e6597b93" width="400">
</p>

# Table of contents

* [About](#about)
* [Prerequisites](#prerequisites)
* [Installation](#installation)
* [Getting started](#getting-started)

## About <a name="about"></a>
**wannierflow** is a user-friendly, in-house developed python-based workflow to automate the construction process of wannier functions. It is mainly used in computational physics, chemistry, or materials science research projects.

The workflow 
1. Generates the input files of VASP, based on a provided POSCAR file
2. Creates the submission file for the whole process
3. Generates the input file of Wannier90, based on the output of VASP
4. Generates a plot of wannier functions on the top of the band structure ontained with VASP, allowing faster quality assessment. 
5. Can recognise missing parts in the process of the calculation and resubmit the necessary steps, without intervention

More details can be found in the Notes.pdf file.

## Prerequisites <a name="prerequisites"></a>
1. Install Python3 (at least 3.6) directly from its website https://www.python.org/downloads/
or via anaconda https://www.anaconda.com/
2. Install package manager for python packages 'pip'
   
   ```
   python -m pip install --upgrade pip
   ```

3. Install the following external python packages using 'pip'
   ```
   pip install pymatgen
   ```
4. Purchase and install VASP directly from its website https://www.vasp.at/
5. Install Wannier90 directly from its website https://wannier.org/ 
6. POSCAR file suitable for the calculation

## Installation <a name="installation"></a>
1. Clone or download the repository
2. Save it at the directory you want to perform the calculation

## Getting started <a name="getting-started"></a>
1. Set all relevant parameters within 'input_parameters.py' according to the description and your needs
2. Modify lines 344-362 of 'vasp_input_hte_cif.py' according to your operating system
3. Run 'vasp_input_hte_cif.py' using python 3
   ```
   python vasp_input_hte_cif.py
   ```
