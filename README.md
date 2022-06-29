# CB8-end-point-calculation

This folder contains all charge models employed in our extensive end-point free energy calculations on the Cucurbit[8]uril host-guest systems.

The AM1-BCC charge scheme performs AM1 optimization and then computes charges by combining AM1 Mulliken charges and BCC corrections.

The two RESP charge schemes follow similar numerical procedures, including B3LYP/6-31G* optimization and then ESP scanning at some ab initio levels to generate the reference data. The difference lies in the level for the ESP scan. RESP-1 follows the traditional HF/6-31G* regime, while the RESP-2 scheme follows a more modern level of B3LYP/def2-TZVPP plus the IEFPCM solvation. The reason for choosing these two levels for ESP scanning is the notable difference between the ESP data at the two levels.

According to ESP analyses, the fitting target (i.e., ESP) in vacuo is significantly different from that in implicit solvent. Thus, the two RESP charge sets produce molecular ESP with significant difference. The corrected semi-empirical charge scheme, AM1-BCC, although fitted with gas-phase HF/6-31G* data, fails to reproduce the HF/6-31G* ESP for the macrocyclic host CB8 but does a better job in reproducing the implicit-solvent results. 

The full text of the manuscript would be released soon. 
