# Phase-Diversity-Reconstruction-code:

This rep contains a Python package that I have written for applying Phase Diversity Reconstruction on Solar Orbiter data. It could be applied on any astronomical data as well. It is for people who are used to IDL, meaning they do not have to worry about passing arguments to the functions when running the code. In the file "main.py", you will have to enter all the parameters of your optical system and the corresponding data. Everything is documented there. You just have to run the main.py file. It lacks the functionalities of a complete python package ([which you can see here](https://github.com/fakahil/PyPD)) but it is enough to have the Zernike polynomials.

It is based on the algorithm described in [Löfdahl and Scharmer. 1994](http://adsabs.harvard.edu/full/1994A&AS..107..243L)

The code requires a pair of focused-defocused images acquired by an optical instrument (telescope or microscope) with a known amount of defocus to retrieve both the wavefront error in the Exit pupil of the system, and the original aberration-free scene under observation.

To test for the robustness of the code, I have tested the algorithm on a MURAM simulation by creating a wavefront to degrade the original data and then retrieve it with the original scene after running the PD code. A check of robustness is done by comparing the original and restored data. This is documented in this [jupyter notebook](https://github.com/fakahil/Phase-Diversity-Reconstruction-code/blob/master/PD_robustness.ipynb)
