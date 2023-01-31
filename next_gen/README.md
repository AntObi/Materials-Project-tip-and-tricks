# Materials Project (next-gen)

This folder will contain some tips and tricks for querying the Materials Project using either `pymatgen.ext.matproj` or [`mp-api`](https://github.com/materialsproject/api). 
## Installation
`mp-api` should already be installed if you have installed `pymatgen`. If not, you can install it through PyPI (https://pypi.org/project/mp-api/) as shown below:

```shell
pip install mp-api
```

## Getting setup

You will need to register on the next-gen Materials Project site (https://materialsproject.org/) and get your API key from the website in order to use the API.

I would first recommend reading through the documentation for the Materials Project (https://docs.materialsproject.org/downloading-data/how-do-i-download-the-materials-project-database) as the explanations and the code examples should be sufficient to get started with making queries with the new API.

## Notebooks

The notebooks in this folder are meant to be used as a reference for how to use the API. They are not meant to be run in order, but rather as a reference for how to use the API. The notebooks are as follows:

* `simple_queries.ipynb`: This notebook shows how to make simple queries to the API. It shows how to query for a single material, a list of materials, and a list of materials with a specific property.
* `saving_queries.ipynb`: This notebook shows how to save the results of a query to a file. It also shows how to load the results of a query from a file.