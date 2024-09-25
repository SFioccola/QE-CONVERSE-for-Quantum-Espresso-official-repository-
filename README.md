# QE-CONVERSE
This is the official Git repository of the QE-CONVERSE code for Quantum-Espresso.  
This current version of the code is compatible with the version 7.2 of Quantum-Espresso package.


## Features
The QE-CONVERSE implement a non-perturbative approach (converse) to compute the orbital magnetization in isolated and periodic systems. The calculation of orbital magnetization allows ab-initio computation of macroscopic properties like the Nuclear Magnetic Resonance (NMR) chemical shifts and the Electronic Paramagnetic Resonance (EPR) g tensor.

* NMR shielding tensors
* EPR g-tensor
* It works only with Norm-conserving pseudopotential with GIPAW reconstruction (https://sites.google.com/site/dceresoli/pseudopotentials)
* LDA and GGA functionals
* isolated and periodic systems

## Build instructions:
1. the Quantum-Espresso package version 7.2 must be previously installed (https://gitlab.com/QEF/q-e/-/releases/qe-7.2). To take advantage of the enhancements in linear algebra operations, the configuration with scaLAPACK package or ELPA library is suggested.
2. ```git clone https://github.com/mammasmias/QE-CONVERSE``` 
3. ```cd QE-CONVERSE```
4. ```chmod +x configure```
5. ```./configure --with-qe-source="QE folder containing make.inc"```
6. ```make```
## How to use it:
run ```./qe-converse.x```

## Directory contents

```/src/```: Contains the source code and the Makefile.  
```/doc/```: Contains the User's manual.  
```/example/```: Contains two directories:  
 ```/EPR/``` about a EPR g tensor and  ```/NMR/``` about a NMR chemical shift calculation. Inside each one there's a Tutorial.wiki file that explain how to perform the calculation step-by-step.
```/benchmarking/``` : Contains the input files used to benchmark the code. Concerns the EPR g tensor calculation of diatomic paramagnetic radicals.
```/application/```: Contains the EPR and NMR calculationsw.
 ## Authors and contributors
S. Fioccola, L. Giacomazzi, D. Ceresoli, N. Richard, A. Hemeryck, L. Martin-Samos

