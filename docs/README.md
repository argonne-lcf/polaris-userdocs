# Polaris User Guide

## Note: Our Polaris documentation is still under development. 

## GPU Hackathon Attendees ##
Please direct questions/issues to your mentor and/or post in the #cluster_support channel in the Hackathon Slack workspace.

## ESP/ECP Users and ALCF Staff ##
Please direct all questions, requests, and feedback to [support@alcf.anl.gov](support@alcf.anl.gov). 

**Please don't submit PRs against this repository.**

## About Polaris
The Polaris software environment is equipped with the HPE Cray programming environment, HPE Performance Cluster Manager (HPCM) system software, and the ability to test programming models, such as OpenMP and SYCL, that will be available on Aurora and the next-generation of DOE’s high performance computing systems. 

Polaris users will also benefit from NVIDIA’s HPC software development kit, a suite of compilers, libraries, and tools for GPU code development. 

## Instructions for building/viewing pages locally 

### Python environment

To build documentation locally, you need a Python environment with `mkdocs` installed. Check that Python 3.6+ is installed:

```
$ python --version
Python 3.8.3
```

Then create a new virtual env to isolate the `mkdocs` installation:
```
$ python -m venv env
$ source env/bin/activate
```

### Git

Using Git ssh. Make sure you add ssh public key to your profile (https cloning to be deprecated soon)
```
$ git clone git@github.com:argonne-lcf/alcf-userguide.git
```

### Installing Mkdocs

To install `mkdocs` in the current environment: 

```
$ cd polaris-userguide
$ make install-dev
```

### Preview the Docs Locally

Run `mkdocs serve` or `make serve` to auto-build and serve the docs for preview in your web browser.
```
$ make serve
```


