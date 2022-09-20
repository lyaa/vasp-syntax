# vasp-highlight README

## Features

Provides syntax support for the Vienna Ab initio Simulation Package (VASP) input files. It is a work in progress but currently supports all 355 INCAR tags and recognizes valid values for each of them. It has initial support for POSCAR (CONTCAR) and KPOINTS (IBZKPT) files.

There are also a few snippets for INCAR files:

|Prefix|Description|
|------|-----------|
|NCORE or KPAR or LREAL| Declare performance optimization settings|
|ISTART or ICHARG| Declare starting parameters|
|ENCUT or ALGO or NELM or EDIFF or PREC| Declare electronic optimization settings|
|LORBIT| Write DOSCAR and lm-decomposed PROCAR|
|ISIF| Determines whether the stress tensor is calculated and which principal degrees-of-freedom are allowed to change in relaxation and molecular dynamics runs. |
|EDIFFG or NSW or IBRION| Declare ionic relaxation parameters|
|LSORBIT| General settings for adding spin orbit coupling. Should be applied after a self consistent run|

### INCAR

![Example of INCAR file](/assets/INCAR.png)

### POSCAR

![Example of POSCAR file](/assets/POSCAR.png)

### KPOINTS

![Example of KPOINTS file](/assets/KPOINTS.png)

## Release Notes

### 1.2.0
Added snippets contributed by @wladerer 

### 1.1.0

Improved support for INCAR files, added support for the following files:

- KPOINTS
- IBZKPT
- POSCAR
- CONTCAR

### 1.0.0

Initial release with support for INCAR files.

---
