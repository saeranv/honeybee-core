![Honeybee](https://www.ladybug.tools/assets/img/honeybee.png)

[![Build Status](https://travis-ci.org/ladybug-tools/honeybee-core.svg?branch=master)](https://travis-ci.org/ladybug-tools/honeybee-core)
[![Coverage Status](https://coveralls.io/repos/github/ladybug-tools/honeybee-core/badge.svg?branch=master)](https://coveralls.io/github/ladybug-tools/honeybee-core)

[![Python 2.7](https://img.shields.io/badge/python-2.7-green.svg)](https://www.python.org/downloads/release/python-270/) [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/) [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)

# honeybee-core

Honeybee is a collection of Python libraries to create, run and visualize
daylight ([RADIANCE](https://radiance-online.org//)) and energy
([EnergyPlus](https://energyplus.net/)/[OpenStudio](https://www.openstudio.net/)) models.

This repository is the core repository that provides honeybee's common functionalities.
To extend these functionalities you should install available Honeybee extensions or write
your own.

Here are a number of frequently used extensions for Honeybee:

- [honeybee-energy](https://github.com/ladybug-tools/honeybee-energy): Adds Energy simulation to Honeybee.
- [honeybee-radiance](https://github.com/ladybug-tools/honeybee-radiance): Adds daylight simulation to Honeybee.


# Installation

To install the core library try:

`pip install -U honeybee-core`

If you want to also include the command line interface try:

`pip install -U honeybee-core[cli]`

To check if Honeybee command line is installed correctly try `honeybee viz` and you
should get a `viiiiiiiiiiiiizzzzzzzzz!` back in response! :bee:


# [API Documentation](https://www.ladybug.tools/honeybee-core/docs/)


## Local Development
1. Clone this repo locally
```console
git clone git@github.com:ladybug-tools/honeybee-core.git

# or

git clone https://github.com/ladybug-tools/honeybee-core.git
```
2. Install dependencies:
```console
cd honeybee-core
pip install -r dev-requirements.txt
pip install -r requirements.txt
```

3. Run Tests:
```console
python -m pytests tests/
```

4. Generate Documentation:
```console
sphinx-apidoc -f -e -d 4 -o ./docs ./honeybee
sphinx-build -b html ./docs ./docs/_build/docs
```
