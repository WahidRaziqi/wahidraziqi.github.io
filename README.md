# wahidraziqi.github.io



## Project description



This project is a personal academic website created for the UBC Master of Data Science program. The site is built with Quarto and published using GitHub Pages.



For Milestone 3, the project includes three computational blog posts:



* **Python:** Exploring the Iris Dataset with Python

* **R:** Exploring the Iris Dataset with R

* **R + Python:** R and Python in One Post using `reticulate`



The Python and R posts use code to load, analyze, and visualize the Iris dataset. The R + Python post demonstrates passing an object between R and Python using `reticulate`. The analysis and figures are generated when the Quarto site is rendered.



## Software versions



This project uses:



* Quarto

* Python 3.14

* R

* `uv` for Python environment management

* `renv` for R environment management



The exact Python package versions are recorded in `uv.lock`.



The exact R package versions are recorded in `renv.lock`.



## How to build the site



Clone the repository and move into the project directory:



```bash

git clone https://github.com/WahidRaziqi/wahidraziqi.github.io.git

cd wahidraziqi.github.io

```



### Python environment



The Python environment is managed with `uv`.



To install the locked Python environment:



```bash

uv sync

```



### R environment



The R environment is managed with `renv`.



Open R from the project directory and run:



```r

renv::restore()

```



### Render the website



From the top-level project directory, run:



```bash

uv run quarto render

```



The generated website is placed in the `docs/` directory.



To view the site locally, open:



```text

docs/index.html

```



## Data sources



The computational posts use the Iris dataset.



The Python post obtains the Iris dataset from scikit-learn:



https://scikit-learn.org/stable/datasets/toy_dataset.html#iris-dataset



The R post uses the built-in `iris` dataset included with R's `datasets` package.



The project requires network access when installing dependencies and when cloning or pushing the repository. The computational analyses themselves use the datasets provided by the Python package and R installation.



## Reproducibility



The Python environment is pinned using:



* `.python-version`

* `pyproject.toml`

* `uv.lock`



The R environment is pinned using:



* `.Rprofile`

* `renv.lock`

* `renv/`



The R package library is not committed to the repository.



## Website



The published website is available through GitHub Pages:



https://WahidRaziqi.github.io/



