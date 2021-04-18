# ncmaps
**ncmaps brings scientific colormaps to ncview.**

[ncview](http://meteora.ucsd.edu/~pierce/ncview_home_page.html) is a legacy, light-weight netcdf viewer that is still in wide use in the geosciences community.

One of the weak points of ncview is its colormaps (e.g. jet), in particular the lack of *scientific* (*aka perceptually uniform*) colormaps.

**ncmap** adds scientific colormaps to the configuration path of ncview, so that your data can be displayed using *viridis*, *inferno*, *cmocean*, and more.

## Installation

 1. Fetch the ncmaps repo from github, alternatively copy the ncmaps file;
 2. Run ncmaps in the terminal (requires Python3);
 3. Define (export) a shell environment variable: `export NCVIEWBASE=${HOME}/.ncmaps`;
 
New colormaps should be available the next time you run `ncview`.

## Supported colormaps
*ncmaps* harvests scientific colormaps from the following python modules:
 * [matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html)
 * [cmocean](https://matplotlib.org/cmocean/)
 * [cmcrameri](https://pypi.org/project/cmcrameri/)

These modules must be installed and accessible to your your python implementation (e.g. via *pip* or *conda*) **before** running ncmaps.
Modules that are not available are skipped.

## Command-line parameters

Running `ncmaps` should be enough in most cases, but check `ncmaps -h`.

## Author
Thomas Lavergne, Norwegian Meteorological Institute

(ncmaps expands https://github.com/samhatfield/ncview-scientific-colour-maps)
