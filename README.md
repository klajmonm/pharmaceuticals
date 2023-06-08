## Pharmaceuticals

# Supporting data for our studies regarding pharmaceuticals

**Optimal gas-phase structures of 16 pharmaceutical molecules**


obtained using conformational analysis in RDKit (http://www.rdkit.org) and further refinement at the DFT/BP86/pVTZ-D3 level. 

To identify the optimal vacuum geometry of an API, it is
essential to start with a thorough conformational analysis. For
this purpose, we first applied a pre-optimization stage using the
tool RDKit115 implemented in AMS, which generated a large set
of 600 or more random conformations of each API and
optimized them at a molecular mechanical level using the
Universal Force Field (UFF).116 A set of API geometries with
the lowest UFF energies (units or dozens of geometries,
depending on the API flexibility) was then re-optimized at a
relatively cheap QM level (DFT/BP86/pVDZ) to obtain more
accurate molecular energies. Geometries with the lowest QM
energy were then compared to conformational information on a
given API available in the literature117−125 and the final selected
geometry was used as an initial guessfor the further COSMO-RS
parametrization calculations.
Having identified the appropriate initial guess of optimum
geometry for each API, we applied the default COSMO-RS
parametrization setup in the ADF program of AMS (the preset
“COSMO-RS Compound”),114 which (i) further refined the
geometry at the DFT/BP86/pVTZ level and (ii) p

Data used in .
