# Hierarchical organization of the FcµR–IgM interface across distinct IgM oligomeric states

This dataset contains processed MD trajectories, topologies, analysis results,
and feature matrices for the FcµR–IgM recognition interface study.

## Dataset structure
.
├── trajectories/
│ ├── WT_prod_fit.xtc
│ ├── D111A_prod_fit.xtc
│ ├── T110A_D111A_prod_fit.xtc
│ └── T60A_S63A_prod_fit.xtc
├── topologies/
│ ├── toppar/
│ ├── WT/
│ ├── D111A/
│ ├── T110A_D111A/
│ └── T60A_S63A/
├── data/
│ ├── WT/
│ ├── D111A/
│ ├── T110A_D111A/
│ └── T60A_S63A/
├── msm/
│ ├── its_k150.npy
│ ├── lags_k150.npy
│ ├── dtraj_k150.npy
│ ├── pcca_membership.npy
│ ├── ck_errors.npy
│ └── eigenvalues.npy
├── tica/
│ ├── system_labels.npy
│ ├── WT_tica.npy
│ ├── D111A_tica.npy
│ ├── T110A_D111A_tica.npy
│ └── T60A_S63A_tica.npy
└── source_file/
├── 7YTE.pdb
├── 7YTC.pdb
├── 7YTD.pdb
├── 7YSG.pdb
├── 8BPE.pdb
├── 8BPF.pdb
└── 8BPG.pdb


## File descriptions
- `trajectories/` – processed MD trajectories (0–200 ns, 100 ps/frame, 2001 frames each)
- `topologies/` – GROMACS inputs and `toppar/` force field
- `data/` – per‑system analysis results (`.xvg`, `.dat`, `.pdb`)
- `msm/` – Markov state model matrices (`.npy`)
- `tica/` – TICA projections (`.npy`)
- `source_file/` – input PDB structures of the seven FcµR–IgM complexes

## Reproducing the analyses
Analysis scripts are maintained in a separate code repository. Please refer to
the associated manuscript or contact the authors for details.
