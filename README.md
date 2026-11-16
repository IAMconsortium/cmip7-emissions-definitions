# CMIP7 Emissions Definitions

Copyright 2026 IIASA and participating modeling teams

[![Code style: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

## Overview

This repo has definitions for the variables used in the CMIP7 emissions datasets.

### Project nomenclature

The folder `definitions` has the definitions and expected units of the variables.

### Workflow

The module `workflow.py` has a function `main(df: pyam.IamDataFrame) -> pyam.IamDataFrame:`.

Per default, this function takes an **IamDataFrame** and returns it without
modifications. [Read the docs](https://pyam-iamc.readthedocs.io) for more information
about the **pyam** package for scenario analysis and data visualization.

**Important**: Do not change the name of the module `workflow.py` or the function `main`
as they are called like this by the Job Execution Service. Details can be found
[here](https://wiki.ece.iiasa.ac.at/wiki/index.php/Scenario_Explorer/Setup#Job_Execution_Service).
