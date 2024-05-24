Design of Near-Perfect Absorptance in Few-Layer WSe2 via Cooperative Enhancement Mechanisms
EKIN GUNES OZAKTAS, SREYAS CHINTAPALLI, SERENE KAMAL, AND SUSANNA M. THON
May 2024

In this repository, we provide the data associated with the aforementioned paper. Referring to the paper figure by figure, the files correspond to the following:

Fig. 1: Fabry_Perot.mat
This contains data corresponding to the study of the Fabry-Perot structure. The RT cell array in the file contains 201 structs corresponding to different cavity thicknesses, and each contains the amplitude and power coefficients.

Fig. 2, 4: Modeling_b_350_w_0_20_100.mat, Modeling_b_350_w_125_25_175.mat, Modeling_b_350_w_200_25_225.mat, Modeling_b_350_w_250_20_350.mat, Modeling_b_400_w_0_20_100.mat, Modeling_b_400_w_140_40_180.mat, Modeling_b_400_w_220_40_260.mat, Modeling_b_400_w_300_20_400.mat 
These contain the study of the modal hybridizations. The naming convention is b_ followed by the value of the period in nm, and then w_ followed by the start, increment, and stop value (all inclusive) in the width sweep.
Each power monitor (Refl, Trans_abs, Trans_ext) contains the wavelength and frequency information (under lambda and f respectively), and also the power coefficient associated with the labeled quantity under T.
Refl is the reflectance from the structure, Trans_abs is T_abs as denoted in the paper, and Trans_ext is T_tot as denoted in the paper. Note that to process these values properly, one must add 1 to all of the raw values from the reflectance monitor and multiply all the values in the transmittance monitors by -1, to correctly account for the directions and the incident light.

Fig 3: Modeling_b_350_20_450_w_40.mat
This file is a period sweep from 350 to 450 nm in increments of 20 nm, at a nanowire width of 40 nm. The data is otherwise structured identically to the width sweeps mentioned above.

Fig 5: Optimization_b_400_w_0_20_100.mat
This file is a width sweep using the full WSe2 material model. The data is structured identically to the width sweeps mentioned above.

Fig 6: Architecture_Comp_Top_Bare.mat, Architecture_Comp_Top_AR.mat, Architecture_Comp_Top_AR_NW.mat, Architecture_Comp_Bottom_BR.mat, Architecture_Comp_Bottom_BR_spacer.mat, Architecture_Comp_Bottom_BR_spacer_NW.mat
These correspond to the comparison of different architectures. The files with "Top" in their name correspond to the enhancement mechanisms being on the top (the side the light comes from), and correspond to designs 1-3 in the paper. AR denotes the presence of an antireflection coating, and NW the presence of a nanowire array, as described in the paper. The data for these is structured identically to the width sweep above, with the exception that now it contains Trans, Refl_abs, and Refl_ext. These correspond to the reflectance monitors needed to calculate only the absorptance in the WSe2 versus the WSe2 and the nanowires. The files with "Bottom" in their name correspond to the enhancement mechanisms being on the bottom (opposite the side the light comes from), and correspond to designs 4-6 in the paper.  BR denotes the presence of a back reflector, and NW the presence of a nanowire array. The data for these is structured identically to the width sweep above.
