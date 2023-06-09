# Pharmaceuticals

## Supporting data for our studies regarding pharmaceuticals:

- Optimal gas-phase structures of 16 pharmaceutical molecules determined using the following approach:
> 1. Conformational analysis: pre-optimization stage using [RDKit](http://www.rdkit.org) as implemented in the [Amsterdam Modeling Suite](https://www.scm.com/) (AMS), which generated a large set of 600 or more random conformations of each API and optimized them at a MM level using the [Universal Force Field](https://doi.org/10.1021/ja00051a040) (UFF).
> 2. A set of API geometries with the lowest UFF energies (units or tens of geometries, depending on the API flexibility) was then re-optimized at a cheaper QM level (DFT/BP86/pVDZ) to obtain more accurate molecular energies.
> 3. Geometries with the lowest QM energy were then compared to conformational information available in the literature ([A1](https://doi.org/10.1016/j.ejps.2020.105273), [A2](https://doi.org/10.1107/S2052520613026711), [A3](https://doi.org/10.1002/jps.21007), [A4](https://doi.org/10.1093/jb/mvj176), [A5](https://doi.org/10.1039/C5NJ01753J), [A6](https://doi.org/10.1016/j.molliq.2015.10.060), [A7](https://doi.org/10.24297/jac.v16i0.8099), [A8](https://doi.org/10.1002/chem.201705954), [A9](https://doi.org/10.1016/j.molstruc.2017.07.031), [A10](https://doi.org/10.1021/mp400132r), [A11](https://doi.org/10.1021/acs.molpharmaceut.8b00818), [A12](https://doi.org/10.1021/cg3000075)).
> 4. The final selected geometry was further refined at the DFT/BP86/pVTZ level as part of the default COSMO-RS-AMS parametrization setup in the [ADF program](https://doi.org/10.1002/jcc.1056) of AMS (the preset “COSMO-RS Compound”).
 
Closer details are given in [Klajmon, M. Purely Predicting the Pharmaceutical Solubility: What to Expect from PC-SAFT and COSMO-RS? *Mol. Pharmaceutics* **2022**, *19*, 4212-4232](https://doi.org/10.1021/acs.molpharmaceut.2c00573).

