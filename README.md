## CEA theme for beamer with LaTeX (2023 recommendations)
Theme is defined in `beamerthemeCEA.sty`.  
Template is `beamerCEA.tex`. 
Required graphics are in `graphics/`.  

### Typefaces
CEA recommends using Arial, but we use the Helvetica typeface, loaded with package `helvet`.
For the math typeface, we also use Helvetica, for a better blending with the text.  
Greeks and symbols are taken from the sans-serif Computer Modern typeface.  
Blackboard letters are set to sans-serif Doublestroke typeface.  
Calligraphic letters are set as Zapf Chancery and scaled with the `mathalfa` package.  

### Misc
The `babel` package with option `french` is not loaded by default in the theme, but included in the template.  
The template includes several classical commands in the preambule; logotypes can be changed here as well. In particular, two different possibilities are given as examples, one adapted to the DEN department, the other to the IRFM laboratory.

### Acknowledgements

This theme is adapted from https://gitlab.com/1a7r0ch3/CEA (previous recommentations).
