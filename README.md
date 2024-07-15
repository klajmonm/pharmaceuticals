# Pharmaceuticals

## Supporting data for our studies regarding pharmaceuticals:

- Optimal gas-phase geometries (.xyz) of 11 drug molecules (see their list below) determined using the following approach:
> 1. Conformational analysis: pre-optimization stage using [RDKit](http://www.rdkit.org) as implemented in the [Amsterdam Modeling Suite](https://www.scm.com/) (AMS), which generated a large set of 600 or more random conformations of each API and optimized them at a MM level using the [Universal Force Field](https://doi.org/10.1021/ja00051a040) (UFF).
> 2. A set of API geometries with the lowest UFF energies (units or tens of geometries, depending on the API flexibility) was then re-optimized at a cheaper QM level (DFT/BP86/pVDZ) to obtain more accurate molecular energies.
> 3. Geometries with the lowest QM energy were then compared to conformational information available in the literature ([A1](https://doi.org/10.1016/j.ejps.2020.105273), [A2](https://doi.org/10.1107/S2052520613026711), [A3](https://doi.org/10.1002/jps.21007), [A4](https://doi.org/10.1093/jb/mvj176), [A5](https://doi.org/10.1039/C5NJ01753J), [A6](https://doi.org/10.1016/j.molliq.2015.10.060), [A7](https://rajpub.com/index.php/jac/article/view/8099), [A8](https://doi.org/10.1002/chem.201705954), [A9](https://doi.org/10.1016/j.molstruc.2017.07.031), [A10](https://doi.org/10.1021/mp400132r), [A11](https://doi.org/10.1021/acs.molpharmaceut.8b00818), [A12](https://doi.org/10.1021/cg3000075)).
> 4. The final selected geometry was further refined at the DFT/BP86/pVTZ level as part of the default COSMO-RS-AMS parametrization setup in the [ADF program](https://doi.org/10.1002/jcc.1056) of AMS (the preset “COSMO-RS Compound”).

Closer details are given in [Klajmon (2022)](https://doi.org/10.1021/acs.molpharmaceut.2c00573).

- COSMO-SAC sigma-profiles (.sigma) of the 11 drugs at their optimal gas-phase geometries:
> Determined from the COSMO surface screening charge densities calculated with [Gaussian 16]([https://gaussian.com/gaussian16/](https://gaussian.com/gaussian16/)) (revision C.01) at the DFT BVP86/TZVP level of theory; the solvation was accounted for using [the conductor-like polarizable continuum model](https://gaussian.com/scrf/) with infinite dielectric limit. (Gaussian specification line:
``` #p BVP86/TZVP scf=tight density=current scrf=cosmors ```). For sigma-profile calculation based on the COSMO surface screening charge densities, we used the [to_sigma.py](https://github.com/usnistgov/COSMOSAC/blob/9388a88d9a9ff7bbc0bbb2e4aa0095aba3e703ff/profiles/to_sigma.py) tool. When using these sigma-profiles, please also cite Gaussian as follows:

```bibtex
@misc{g16,
author={M. J. Frisch and G. W. Trucks and H. B. Schlegel and G. E. Scuseria and M. A. Robb and J. R. Cheeseman and G. Scalmani and V. Barone and G. A. Petersson and H. Nakatsuji and X. Li and M. Caricato and A. V. Marenich and J. Bloino and B. G. Janesko and R. Gomperts and B. Mennucci and H. P. Hratchian and J. V. Ortiz and A. F. Izmaylov and J. L. Sonnenberg and D. Williams-Young and F. Ding and F. Lipparini and F. Egidi and J. Goings and B. Peng and A. Petrone and T. Henderson and D. Ranasinghe and V. G. Zakrzewski and J. Gao and N. Rega and G. Zheng and W. Liang and M. Hada and M. Ehara and K. Toyota and R. Fukuda and J. Hasegawa and M. Ishida and T. Nakajima and Y. Honda and O. Kitao and H. Nakai and T. Vreven and K. Throssell and Montgomery, {Jr.}, J. A. and J. E. Peralta and F. Ogliaro and M. J. Bearpark and J. J. Heyd and E. N. Brothers and K. N. Kudin and V. N. Staroverov and T. A. Keith and R. Kobayashi and J. Normand and K. Raghavachari and A. P. Rendell and J. C. Burant and S. S. Iyengar and J. Tomasi and M. Cossi and J. M. Millam and M. Klene and C. Adamo and R. Cammi and J. W. Ochterski and R. L. Martin and K. Morokuma and O. Farkas and J. B. Foresman and D. J. Fox},
title={Gaussian˜16 {R}evision {C}.01},
year={2016},
note={Gaussian Inc. Wallingford CT}
} 
```

## List of APIs:

- carbamazepine (CBZ)
- griseofulvin (GSF)
- ibuprofen (IBP)
- indomethacin
- nifedipine
- naproxen
- paracetamol
- ribavirin
- simvastatin
- tolbutamide
- valsartan
