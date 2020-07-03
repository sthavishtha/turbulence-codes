# Open source codes for turbulent flows
A curated list of some open source frameworks, libraries and softwares for turbulent flow simulations. This list includes solvers for turbulent multiphase, turbulent reacting flows, turbulent convection and turbulent atmospheric physics as well. This list is by no means complete. So if you would like me to add something, please send me a link to sthavishthabr@gmail.com or perform a pull request. 

<span style="color:red"> ----------------- To be updated -------------- </span>

---------------------------
## Numerical frameworks (physics-based)
* [spectralDNS](https://github.com/spectralDNS/spectralDNS) [[1](#spectralDNS)] - a parallelized numerical solver employing spectral Galerkin methods for Direct numerical simulations (DNS) in triply periodic domains. Written in Python and uses NumPy, mpi4py and pyFFTW. Developed at the Department of Mathematics, University of Oslo [webpage](http://folk.uio.no/mikaem/research/spectraldns.html).  
* [STREAMmS](https://github.com/matteobernardini/STREAmS) [[2](#streams)] - a parallelized numerical framework (available in both CPU and CUDA GPU) in FORTRAN for performing DNS simulations of compressible turbulent flows (by solving the fully compressible Navier-Stokes equations (NSE)). Developed at the [Sapienza University of Rome](https://www.uniroma1.it/en/pagina-strutturale/home) and [Delft University of Technology](https://www.tudelft.nl/en/). 
* [freeCappuccino](https://github.com/nikola-m/freeCappuccino) [[3](#freeCappuccino_1), [4](#freeCappuccino_2)] - a fully unstructured finite volume spatially discretized parralelized numerical code written in FORTRAN. Developed at the [University of Belgrade](http://www.bg.ac.rs/en/). 
* [channel-f90-mpi](https://github.com/davecats/channel-f90-mpi) [[](#channel-f90-mpi)] - an MPI parallelized numerical code in FORTRAN for performing DNS simulations of an incompressible turbulent channel flow. 
* [Xcompact3D](https://github.com/xcompact3d/Incompact3d) [[5](#xcompact3d)] - an MPI parallelized numerical framework in FORTRAN 90 & 95 which solves the incompressible NSE. Uses high-order compact finite differences on a cartesian mesh. Developed at the [Department of Astronautics](https://www.imperial.ac.uk/aeronautics/), [Imperial College London](https://www.imperial.ac.uk/).
* [WABBIT](https://github.com/adaptive-cfd/WABBIT) [[6]((#wabbit)] - (W)avelet (A)daptive (B)lock-(B)ased solver for (I)nteractions with (T)urbulence. An MPI parallelized numerical framework using block-based adaptive grids. High-order central finite differences are used for numerical discretization. Developed at the [Technische Universität Berlin](https://www.tu.berlin/en/). 
* [NALU](https://github.com/NaluCFD/Nalu) [[7](#nalu)] - a parallelized numerical framework for unstructured meshes which uses control volume finite element (CVFEM) and edge-based vertex centered (EBVC) discretization approaches. Supports LES, RANS and DES turbulence models. Developed at the [Sandia National laboratories](https://www.sandia.gov/). 
* [T-Flows](https://github.com/DelNov/T-Flows) [[](#tflows)] - a parallelized numerical framework for unstructured meshes using cell centered finite volume (FVM) numerical discretization. Also supports RANS, LES and hybrid LES/RANS turbulent models. Developed originally at the [Delft University of Technology](https://www.tudelft.nl/en/).
* [LESGO](https://github.com/lesgo-jhu/lesgo) [[8](#lesgo)] - a FORTRAN MPI parallelized pseudo-spectral large eddy simulation (LES) code for solving the filtered NSE. Includes capabilities for wind turbine modeling, level set immersed boundary methods and atmospheric boundary layer flows as well. Developed at the [Turbulence research group](https://pages.jh.edu/~cmeneve1/) at [John Hopkins University](https://www.jhu.edu/). 
* [HAMeRS](https://github.com/mlwong/HAMeRS) [] - Hydrodynamics Adaptive Mesh Refinement Simulator. An MPI parallellelized C++ numerical solver for the compressible NSE with patch-based adaptive mesh refinement (AMR). Utilizes high-order conservative shock and interface capturing Weighted Compact Nonlinear Schemes (WCNS). Developed by the [Flow Physics and Aerocoustics laboratory](https://fpal.stanford.edu/), [Department of Aeronautics and Astronautics](https://aa.stanford.edu/) at [Stanford University](https://www.stanford.edu/). 
* [PENCIL](https://github.com/pencil-code/pencil-code) [[9](#pencil_1), [10](#pencil_2)] - a FORTRAN parallelized high-order finite difference code originally devloped for weakly compressible astrophysical magnetohydrodynamic turbulence. Capabilities for simulating turbulent combustion [(paper)](https://doi.org/10.1016/j.jcp.2010.08.028), turbulent multiphase [(paper)](https://doi.org/10.1017/S0022112010002946), turbulent convection to name a few exist as well. Developed at [NORDITA - Nordic Institute for Theoretical Physics](https://www.nordita.org/) along with contributors from several leading institutions around the world. 
* [nsCouette](https://github.com/ElsevierSoftwareX/SOFTX_2019_225) [[11](#nscouette)] - a hybrid OpenMP-MPI parallelized code in FORTRAN for perfoming DNS simulations of turbulent Taylor-Couette flow. An optional feature of solving for the temperature equation (thermal convective flow) also exists. Uses high-order explicit finite differences. Developed at [ZARM](https://www.zarm.uni-bremen.de/en/), [Universit\"at Bremen](https://www.uni-bremen.de/) and [Max Planck Institute for Dynamics and Self-Organization](https://www.ds.mpg.de/en). 
* 

* AFID, AFID-GPU
* SU2
* OpenFOAM
* Nek5000
* ISAAC
* Openflower
* CodeSaturne
* PyFR
* HiFiLES (https://hifiles.stanford.edu/)
* PyCLES (https://climate-dynamics.org/pycles-a-new-open-source-atmospheric-les-code/)

---------------------------
## Numerical frameworks (data-driven)


---------------------------
## Comparitive studies of some open-source codes
* AFiD vs Nek5000 vs GOLDFUN vs OpenFOAM in turbulent convection (https://doi.org/10.1016/j.compfluid.2018.01.010)
* Nek5000 vs OpenFOAM (https://www.mcs.anl.gov/~fischer/nek5000/sprague_nek5000_dec2010.pdf)
* OpenFOAM vs ParMOON (https://doi.org/10.1016/j.compag.2020.105546)

---------------------------
## Miscellaneous codes for post-processing and analysis
* Eddylicious (https://doi.org/10.1016/j.softx.2018.04.001)
* PyConTurb (10.1088/1742-6596/1037/6/062032)

---------------
## References
1. <a name="spectralDNS"></a> Mortensen, M. and Langtangen, H.P., _High performance Python for direct numerical simulations of turbulent flows_, Computer Physics Communications, Vol. 203, pp. 53-65, 2016. [Link](https://doi.org/10.1016/j.cpc.2016.02.005)
2. <a name="streams"></a> Bernardini, M., Modesti, D., Salvadore, F. and Pirozzoli, S., _STREAmS: a high-fidelity accelerated solver for direct numerical simulation of compressible turbulent flows_, arXiv preprint, 2020. [Link](https://arxiv.org/abs/2004.02276)
3. <a name="freeCappuccino_1"></a> Mirkov, N., Vidanovi{\'{c}}, N., Kastratovi{\'{c}}, G., _freeCappuccino - An Open Source Software Library for Computational Continuum Mechanics_, Proceedings of the International Conference of Experimental and Numerical Investigations and New Technologies, Springer International Publishing, pp. 137-147, 2019. [Link](10.1007/978-3-319-99620-2_11) 
4. <a name="freeCappuccino_2"></a> Mirkov, N., Rašuo, B., Kenjereš, S., _On the improved finite volume procedure for simulation of turbulent flows over real complex terrains_, Journal of Computational Physics, Vol. 297, pp.18-45, 2015. [Link](https://doi.org/10.1016/j.jcp.2015.02.001)
5. <a name="xcompact3d"></a> Bartholomew, P., Deskos, G., Frantz, R.A.S., Schuch, F.N., Lamballais, E., Laizet, S., _Xcompact3D: An open-source framework for solving turbulence problems on a Cartesian mesh_, SoftwareX, Vol. 12, 100550, 2020. [Link](https://doi.org/10.1016/j.softx.2020.100550)
6. <a name="wabbit"></a> Sroka, M., Engels, T., Krah, P., Mutzel, S., Schneider, K. and Reiss, J., _An Open and Parallel Multiresolution Framework Using Block-Based Adaptive Grids_, Proceedings of the Active Flow and Combustion Control, Springer International Publishing, pp. 305 - 319, 2019. [Link](https://doi.org/10.1016/j.softx.2020.100550)
7. <a name="nalu"></a> Domino, S., _Sierra Low Mach Module: Nalu Theory Manual 1.0_, SAND2015-3107W, Sandia National Laboratories Unclassified Unlimited Release (UUR), 2015.
8. <a name="lesgo"></a> [Official website of LESGO](https://lesgo.me.jhu.edu/)
9. <a name="pencil_1"></a> Wikipedia contributors, _Pencil Code_, Wikipedia, The Free Encyclopedia, 17 June 2020. [Link](https://en.wikipedia.org/w/index.php?title=Pencil_Code&oldid=963016141)
10. <a name="pencil_2"></a> [Official website of PENCIL](http://pencil-code.nordita.org/) 
11. <a name="nscouette"></a> López, J.M., Feldmann, D., Rampp, M., Vela-Martín, A., Shi, L. and Avila, M., _nsCouette – A high-performance code for direct numerical simulations of turbulent Taylor–Couette flow_, SoftwareX, Vol. 11, 100395, 2020. [Link](https://doi.org/10.1016/j.softx.2019.100395)
