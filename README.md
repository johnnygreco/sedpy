sedpy
======

Modules for storing and operating on astronomical source spectral energy distributions.

installation & setup:

1. Download code to some directory 'sdir'. 
2. cp any desired filters from the k_correct filter directory to
   'sdir'/data/filters/
   
Description:
- `observate.py` has methods for generating synthetic photometry through
  any filters, and classes for dealing with filters
  generally. Functionality for spectra is being added slowly. With a
  huge debt to Mike Blanton's k_correct code .
  
- `attenuation.py` contains dust attenuation methods (very
  preliminary).

- `extinction.py` contains classes for a detailed modeling of
  extinction curves, following the Fitzpatrick and Massa parameterizations.

- `modelgrid.py` is a module with classes for the storage and
  interpolation of model SEDs (using numpy structured arrays, usually,
  and Delaunay triangulation)

- `photometer.py` has some basic aperture photometry algorithms

- `yanny.py` (from Erin Sheldon) is for reading filter curves.
