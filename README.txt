%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%    Written on 04/20/2020                   %%%
%%%    For more information or any question,   %%%
%%%    please contact                          %%%
%%%    corresponding author Mathieu Bouffard   %%%
%%%    at bouffard.mathieu@gmail.com           %%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%



This file contains all necessary information to reproduce the figures and quantitative results in our paper "Convective erosion of a
primordial stratification atop Earth’s core" published in Geophysical
Research Letters.


We provide all the data used to obtain our quantitative results on erosion. For all simulations, we provide the time evolution of the layer thickness. These are contained in arrays called data_caseX_Ek_XX_RaT_XX_RaC_XX.mat that can be opened with Matlab (load data_caseX_Ek_XX_RaT_XX_RAC_XX.mat). Note that, in the files names,
the Rayleigh numbers are non-dimensionalized using the viscous time
as implemented in the PARODY code. These arrays can be found
in the repository /DATA_allruns and contain

1) A first column for the time (in viscous units)
2) A second column for the thickness of the layer,
calculated using the Matlab routine calc_thickness_from_comp.m
attached.
3) A third column giving the total kinetic energy in the shell.
4) In some cases, we added extra columns: a fourth one containing the
kinetic energy in the convective region only, and a fifth one
containing the poloidal kinetic energy. Because using either one of
these velocities did not improve the scaling law in our paper, we
focused on the total kinetic energy only (column 3) and we stopped calculating
columns 4 and 5 for the rest of the simulations which therefore only
possess 3 columns.


Figures 3 and 4 of the main text, as well as Figures S2, S5-S9 were
obtained using the data_caseX_Ek_XX_RaT_XX_RaC_XX.mat files.
The visualization routines are located in the folder /Figures. 
