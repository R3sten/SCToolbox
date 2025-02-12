# Scientific Computing Toolbox

![Tests](https://github.com/R3sten/SCToolbox/blob/main/.github/workflows/tests.yml/badge.svg)

# Commands used during project creation:

python -m venv venv

source venv/bin/activate

pip install -r requirements.txt

<!-- create pakage in editable mode -->

pip install -e .

<!-- --- -->

# Testing:

pip install -r requirements_dev.txt

## Type checking:

mypy src

flake8 src

## Actual test:

pytest

<!-- Python interpreters need to be installed before -->
<!--
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
-->

sudo apt install python3.10 python3.11 python3.12 python3.13

tox

<!-- dopo un po di fatica adesso il codice gira con successo in qualsiasi enviroment :)
step successivo adesso è far si che funzioni su qualsiasi macchina
ho gia avuto troppe esperienze in passato in cui questo non avveniva, preferisco non passare
l'esame ma sapere che il mio codice è testabile e riproducibile -->
