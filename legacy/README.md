# Materials Project (legacy)

This folder will contains tips and tricks for using the legacy version of the materials project (https://legacy.materialsproject.org)

## Getting set up
[`Pymatgen`](https://pymatgen.org/installation.html) will be needed to query the legacy version of the materials project

1. Sign up for the [materials project](https://legacy.materialsproject.org)
2. Add your API key to your pmgrc.yaml file: `pmg config --add PMG_MAPI_KEY <USER_API_KEY>`

## Notebooks

* `simple_queries.ipynb` - This notebook is used to demonstrate how to query the materials project using MongoDB syntax.
* `querying_properties.ipynb` - This notebook is used to demonstrate the `has` criteria for querying particular properties of the materials project.
* `phonons.ipynb` - This notebook uses the `get_phonon_dos_by_material_id` method to show how to obtain the phonon density of states for a material in the materials project
