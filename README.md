# Jet-Analysis-Module
Developing a module for preprocessing, PIV, post-processing and analysis of jets, with *an aim to quantify key parameters from experimental data like entrainment rates, spreading angle, self-similarity (planar or axisymmetric jets)*. Upon completion the code can be extended to include other parameters like diffusivity.

## Main steps of the project :

1. __Getting familiar with data acquisition and post processing__  
    * Post proceesing sample data from ![2D jet example](https://github.com/alexlib/2D_jet_example), and Experimental Database(http://piv.de/uncertainty/?p=64)
    * Preprocessing PIV images using local tracer particle density to distinguish between fluid entrained in the jet from the surrounding
    * Processing unmasked and masked PIV images and comparing their results

2. __Reading, understanding and deriving the formulas for self-similarity and entrainment as a function of distance__:
    * Chapter 5 Free shear flows from Turbulent Flows by Stephen B. Pope
    * Chapter 5 Exact solutions of Navier-Stokes Equations from Boundary Layer Theory by Hermann Schlichting
    * Chapter 4 Boundary Free Shear Flows from A First Course in Turbulence from Tennekes and Lumley
    * Chapter 3 Solutions of The Newtonian Viscous-Flow Equations from Viscous Fluid Flow by Frank M. White
    * "Mechanics of the Turbulent-Nonturbulent Interface of a Jet" by J. Westerweel, C. Fukushima, J. M. Pedersen, and J. C. R. Hunt Phys. Rev. Lett. 95, 174501 – Published 20 October 2005; Erratum Phys. Rev. Lett. 95, 199902 (2005)
  
3. __Implementing the above formulas in Python, using textbook examples and data from above links for verification__

4. __Testing the code using different sets of data and flow conditions obtained from literature to make the code universal and applicable in different scenarios__, 
The matrix on this website will be used to guide the search for relevant results in different flow conditions(http://piv.de/uncertainty/?page_id=44)

5. __Based on the success of the 2D code, it will be extended to 3D to incorporate PTV results as well__
    * Using the technique mentioned ![on this website](https://ronshnapp.wordpress.com/2019/02/20/3d-ptv-demo-turbulent-jet/) data will be analyzed from ![here](https://figshare.com/articles/3D-PTV_Demo_-_Turbulent_Jet/7754834?file=14441249).
    * The 2D algorithm will then be modified and incorporated in the OpenPTV codes
    * The final 3D code will also be tested on flow conditions similar to the 2D case

