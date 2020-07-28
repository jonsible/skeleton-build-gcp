# Cookiecutter Ansible

[![Build Status](https://travis-ci.com/jonsible/skeleton-build.svg?branch=master)](https://travis-ci.com/jonsible/skeleton-build)

Cookiecutter template for a Ansible role with Molecule testing.

## Features

* Travis-CI: Ready for Travis Continuous Integration testing
* Ansible Galaxy: Ready for deployment to Ansible Galaxy
* Cookiecutter: https://github.com/audreyr/cookiecutter

## Quickstart

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)
```
    pip install -U cookiecutter
```
Generate a Python package project::
```
    cookiecutter https://github.com/jonsible/skeleton-build.git
```

Files you should edit :

```
defaults/*
files/*
molecule/*
tasks/
  source/
    os_specific/*
    install.yml
  config.yml
vars/*
```

## License

GPL-3.0-or-later