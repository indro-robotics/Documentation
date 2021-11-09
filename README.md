# Documentation

This repository contains documentation for Indro Robotics software and products. 

## Contributing to the documentation

Please be sure to read the below sections carefully before contributing.

The site is built using [Sphinx](https://www.sphinx-doc.org/en/master/), and more particularly using [Sphinx multiversion](https://holzhaus.github.io/sphinx-multiversion/master/index.html).

### Installing prerequisites

```
pip3 install --user --upgrade -r requirements.txt
```

### Source structure

The source files for the site are all located under the `source` subdirectory.
the source directory also contains the config files and directory for css modifications.


### Building the site

ReadTheDocs requires a .readthedocs.yaml file that configures it and builds the site. the yaml file points to the config file inside of the source directory.

the config file needs the static directory to be on the same level when compiled

To build the site locally just using sphinx, you must move the config file and the static folder outside of the source directory to the root directory. then type `make html` at the top-level of the repository.



