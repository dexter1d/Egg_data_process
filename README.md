# Egg_data_process
This file guides user to reproduce the results reported in the following study:
Hyperspectral imaging dataset for advancing non-destructive pre-incubation
fertility prediction and structural evaluation of chicken eggs.
Spectra visualization
• Remove all columns except spectral variables from the “spectra and reference
parameters” dataset file (.csv format).
• Upload the file in “Spectra_Visualization_Dataset” and run the code.
Correlation analysis of mass, major, and minor diameters
• Remove all columns except target variables- Mass (g), Major dia (mm), and Minor dia
(mm).
• Upload the file in “Spectra_Visualization_Dataset” and run the code.
Data partitioning
• Upload “spectra and reference parameters” csv file into
“Data_partitioning_into_Cal_Val_and_Test_sets.ipynb” for data partitioning into
calibration, validation, and test sets.
• For classification based on fertility information user needs to run *Stratified sampling
(for fertility classification)* section of the same code file. Follow directions in the code.
PLSR model development for yolk mass
• Remove extra columns from the partitioned data sets: Remove “Sample ID”, “Mass”,
“Major dia”, “Fertilty ”, “Thickness”, “Shell strength”.
• Rename the “Thickness (mm)” column as “Ref” in all sets.
• Run the PLSR_Model_Dataset code and change files paths accordingly.
PLS-DA model development for fertility classification
• Remove the “Sample ID” column from the all the partitioned data sets.
• Rename the “Fertility status” column as “Ref” in all sets.
• Run the PLS_DA_Fertility_model code and change files paths accordingly.
