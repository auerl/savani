# SAVANI

![Scheme](paraview_scene.png =250x)

## Model Description

This is a distributable version of our tomography model SAVANI. 
ascii_reg_grd_1deg contains a version of savani that is expanded on
a 1° by 1° regular grid, ascii_var_grd contains. Please see grid.info
for the exact definition of the inversion grid. 

The columns in each file correspond to:

```
longitude, latitude, depth[km], param
```

With depth being the depth of the center of each layer in [km]
and param being either Voigt average dln(v_s)[%] w.r.t. PREM with 
`v_s = sqrt((2*(v_sv)^2 + (v_sh)^2)/3)`, the anisotropic parameter
`xi=(v_sv/v_sv)^2` or absolute vertical and horizontally polarized
wavespeeds `v_sv[m/s]` and `v_sh[m/s]`.

The folder shansyn contains spherical harmonic expansions of 
dln(v_s) and xi, to be read with Thorsten Beckers spherical harmonic
toolbox shansyn: http://geodynamics.usc.edu/~becker/sdata.html

## Publication

Savani: a variable-resolution whole-mantle model of anisotropic 
shear-velocity variations based on multiple datasets, 
Auer, L., Boschi , L., Becker, T. W., Nissen-Meyer, T. and Giardini, D.
J. Geophys. Res., 2014. doi:10.1002/2013JB010773
