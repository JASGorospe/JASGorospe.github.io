# My Github Page

See page at: https://jasgorospe.github.io/

## Overview
This repository contains the quarto project and requirements needed to make my personal github page. The site contians a brief bio as well as blog posts related to my studies. The rendered project can be found in the docs/ directory. Blog posts and corresponding data are in the post/ directory.

## System Requirements
The following software is required to reproduce the project locally:

* R 4.6.1
* quarto 1.10.18
* uv 0.12.5
* Python 3.14.7 (optional, available through uv)

_This project was developed with MacOS Sequoia 15.7.9 and has not been tested on other operating systems_

## Build Instructions
Steps to recreate this project locally:

1. Download the repository
```bash
git clone git@github.com:JASGorospe/JASGorospe.github.io.git
cd JASGorospe.github.io
```

2. Rebuild Python and R environments

To generate and activate a Python virtual environment from the pyproject.toml file.
```bash
uv sync
```

To recreate and activate the R virtual environment from the renv.lock file.
```r
renv::restore()
```

3. Generate and view the site using Quarto
```bash
uv run quarto render
uv run quarto preview
```

The rendered site is stored in the `docs\` directory. Use `quarto preview` to view the rendered site before publishing.

## Data Sources
Data used in the blog posts is reusable under Creative Commons licensing (see posts for specifics). 

CSVs for the World Development Indicator and Environment and Natural Resources data are provided alongside their respective blog post files. The world dataset comes loaded with the `maps` package for R.



