# Pharmaceuticals

## Supporting data for our studies regarding pharmaceuticals:

- Optimal gas-phase geometries (.xyz) of 11 drug molecules determined using the following approach:
> 1. Conformational analysis: pre-optimization stage using [RDKit](http://www.rdkit.org) as implemented in the [Amsterdam Modeling Suite](https://www.scm.com/) (AMS), which generated a large set of 600 or more random conformations of each API and optimized them at a MM level using the [Universal Force Field](https://doi.org/10.1021/ja00051a040) (UFF).
> 2. A set of API geometries with the lowest UFF energies (units or tens of geometries, depending on the API flexibility) was then re-optimized at a cheaper QM level (DFT/BP86/pVDZ) to obtain more accurate molecular energies.
> 3. Geometries with the lowest QM energy were then compared to conformational information available in the literature ([A1](https://doi.org/10.1016/j.ejps.2020.105273), [A2](https://doi.org/10.1107/S2052520613026711), [A3](https://doi.org/10.1002/jps.21007), [A4](https://doi.org/10.1093/jb/mvj176), [A5](https://doi.org/10.1039/C5NJ01753J), [A6](https://doi.org/10.1016/j.molliq.2015.10.060), [A7](https://rajpub.com/index.php/jac/article/view/8099), [A8](https://doi.org/10.1002/chem.201705954), [A9](https://doi.org/10.1016/j.molstruc.2017.07.031), [A10](https://doi.org/10.1021/mp400132r), [A11](https://doi.org/10.1021/acs.molpharmaceut.8b00818), [A12](https://doi.org/10.1021/cg3000075)).
> 4. The final selected geometry was further refined at the DFT/BP86/pVTZ level as part of the default COSMO-RS-AMS parametrization setup in the [ADF program](https://doi.org/10.1002/jcc.1056) of AMS (the preset “COSMO-RS Compound”).

Closer details are given in [Klajmon (2022)](https://doi.org/10.1021/acs.molpharmaceut.2c00573).

- COSMO-SAC sigma-profiles (.sigma) of the 11 drugs at their optimal gas-phase geometries:
> Determined from the COSMO surface screening charge densities calculated with [Gaussian 16](https://gaussian.com/gaussian16/) (revision C.01) (Frisch *et al.*, 2019) at the DFT BVP86/TZVP level of theory; the solvation was accounted for using [the conductor-like polarizable continuum model](https://gaussian.com/scrf/) with infinite dielectric limit. Gaussian specification line:
``` **#p BVP86/TZVP scf=tight density=current scrf=cosmors** ```. For sigma-profile calculation based on the COSMO surface screening charge densities, we used the [to_sigma.py](https://github.com/usnistgov/COSMOSAC/blob/9388a88d9a9ff7bbc0bbb2e4aa0095aba3e703ff/profiles/to_sigma.py) tool.

Acronyms: CBZ = carbamazepine; GSF = griseofulvin; IBP = ibuprofen; IMC = indomethacin; NIF = nifedipine; NPX = naproxen; PCM = paracetamol; RBV = ribavirin; SIM = simvastatin; TBA = tolbutamide; VST = valsartan

### Reference
> (Frisch *et al.*, 2019) M. J. Frisch, G. W. Trucks, H. B. Schlegel, G. E. Scuseria, M. A. Robb, J. R. Cheeseman, G. Scalmani, V. Barone, G. A. Petersson, H. Nakatsuji, X. Li, M. Caricato, A. V. Marenich, J. Bloino, B. G. Janesko, R. Gomperts, B. Mennucci, H. P. Hratchian, J. V. Ortiz, A. F. Izmaylov, J. L. Sonnenberg, D. Williams-Young, F. Ding, F. Lipparini, F. Egidi, J. Goings, B. Peng, A. Petrone, T. Henderson, D. Ranasinghe, V. G. Zakrzewski, J. Gao, N. Rega, G. Zheng, W. Liang, M. Hada, M. Ehara, K. Toyota, R. Fukuda, J. Hasegawa, M. Ishida, T. Nakajima, Y. Honda, O. Kitao, H. Nakai, T. Vreven, K. Throssell, J. A. Montgomery, Jr., J. E. Peralta, F. Ogliaro, M. J. Bearpark, J. J. Heyd, E. N. Brothers, K. N. Kudin, V. N. Staroverov, T. A. Keith, R. Kobayashi, J. Normand, K. Raghavachari, A. P. Rendell, J. C. Burant, S. S. Iyengar, J. Tomasi, M. Cossi, J. M. Millam, M. Klene, C. Adamo, R. Cammi, J. W. Ochterski, R. L. Martin, K. Morokuma, O. Farkas, J. B. Foresman, and D. J. Fox. Gaussian 16, Revision C.01; Gaussian, Inc., Wallingford CT, 2019.
