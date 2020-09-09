# Phase-Diversity-Reconstruction-code:

This rep contains a Python module that I have written for applying Phase Diversity Reconstruction on Solar Orbiter data. It could be applied on any astronomical data as well.

It is based on the algorithm described in [Löfdahl and Scharmer. 1994](http://adsabs.harvard.edu/full/1994A&AS..107..243L)

The code requires a pair of focused-defocused images acquired by an optical instrument (telescope or microscope) with a known amount of defocus to retrieve both the wavefront error in the Exit pupil of the system, and the original aberration-free scene under observation.

In the file "main.py", you will have to enter all the parameters of your optical system and the corresponding data. Everything is documented there.

The code will be under constant improvement and including jupyter notebooks is also foreseen. Turning it into a package that could be installed will be done once the code is finished.
