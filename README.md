# High-b-value-DWI-denoising
Deep learning based denoising can improve signal-to-noise ratio in high b-value diffusion imaging with reduced acquisition time. We applied deep learning based denoising method on retrospective and prospective high b-value DWI. Unsharp masking used during testing to emphasize medium contrast details.

**Prepare training data**
Retrospective study:
$ python Generate_patches_for_retrospective_DWI.ipynb
Clean patches are extracted from 'training_data/sub-TCRc007/ses-1/dwi' and saved in 'data/npy_data'.

Prospective study:
$ python Generate_patches_prospective_DWI.ipynb
Clean patches are extracted from 'Training_datab3000/04032021/processed' and saved in 'data/npy_data'.

**Train and test**
$ python 

**Test**

**Results**
