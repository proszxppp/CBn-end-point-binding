# CBn-end-point-binding

This folder is the official data repository of our recent paper on large-scale end-point free energy calculations on the Cucurbit[n]uril (n=7 or 8) host-guest systems, https://doi.org/10.1016/j.molliq.2024.125245.  

The paper is built on another paper by us focusing on a detailed yet general inspection of dynamic behaviors produced by general-purpose force fields, see https://github.com/proszxppp/host-dynamics for details. The 7-unit and 8-unit hosts exhibit similar dynamic behaivors under GAFF2, but noticeable differences are identified under GAFF, which is related to the intrinsic flexibility of the host ring. Whether this difference between host dynamics would lead to significant accuracy variations in end-point free energy calculations is the main topic investigated in this work.  

For reusing/reproducing usages, we share the parameter files and initial conditions for complexes. 

The atomic-charge files in the mol2 format for the CBn hosts and the drug-like guests binding to them can be found in the folders named charge. 

The docking-produced initial conditions of host-guest complexes are put in folders with the docking keyword. When reusing these data, please combine the host and guest coordinates into a single file to make the bound complex. 

End-point sampling parameters include the constant-volume heating in 120 ps, NPT equilibration for 1 ns, and 200 ns unbiased sampling in the host-guest and unbound guest states and 20000 ns for the unbound host state, with a sampling interval of 10 ps. 

We additionally provide the binding energetics as an editable docx file for the supporting information, which enables the knowledgeable end-user to quickly assess the performance of the GAFF derivatives in the MM/GBSA approach by classifying the guests according to their chemical features so as to identify weaknesses and strengths of the force field.

