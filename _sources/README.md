<img src="notebooks/images/thumbnail.png" alt="thumbnail" width="300"/>

# Radiative Feedback Cookbook

[![nightly-build](https://github.com/ProjectPythia/radiative-feedback-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/radiative-feedback-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/radiative-feedback-cookbook/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/810464558.svg)](https://zenodo.org/badge/latestdoi/810464558)

This Project Pythia Cookbook explores the fundamental science and practice of radiative feedback analysis applied to climate model output.

## Motivation

There are several well-established methods for quantifying radiative feedbacks from climate model output, and these have been widely used in the scientific literature. However, a comprehensive set of tutorials representing best practices for implementing these methods has been lacking, forcing new practioners to "reinvent the wheel" and piece together the implementation details from sometimes incomplete descriptions in the primary literature.

This Cookbook aims to fill this gap by collecting a verbose set of tutorials that take the reader through some of the basic theory and implementation details, with plentiful example code that can be easily adapted to new datasets and new research applications. The examples will skew heavily toward the method of _radiative kernels_, with some comparison to other methods. 

## Authors

[Ana Castaneda Montoya](https://github.com/anacmontoya), [Ty Janoski](https://github.com/tyfolino), [Robert Ford](https://github.com/r-ford), [Brian Rose](https://github.com/brian-rose), and [Rachel Tam](https://github.com/rytam2)

### Contributors

<a href="https://github.com/ProjectPythia/radiative-feedback-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/radiative-feedback-cookbook" />
</a>

## Structure

This Cookbook is organized as follows:

### Foundations

This section takes the reader through some of the basic ideas and provides an overview of the mathematical theory underlying the radiative kernel method.

### Feedback Analysis

This section links the theory to the practice by demonstrating the detailed implementation of some radiative feedback calculations.

### Simplifying Calculations

This section gives more practical example code for carrying out feedback calculations on CMIP6 data, making use of some specialized software packages.

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/radiative-feedback-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/radiative-feedback-cookbook.git
   ```

1. Move into the `radiative-feedback-cookbook` directory
   ```bash
   cd radiative-feedback-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate feedback-cookbook-dev
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
