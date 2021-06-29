# High-b-value-DWI-denoising
Deep learning based denoising can improve signal-to-noise ratio in high b-value diffusion imaging with reduced acquisition time. We applied deep learning based denoising method on retrospective and prospective high b-value DWI with b-value>=3000s/mm<sup>2</sup>.The base network architecture, we adpated from the  keras implemention of the paper <Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising>.We used unsharp masking after denoising to preserve the modest details.

**Prepare training data**<br />
Retrospective study:<br />
$ python Generate_patches_for_retrospective_DWI.ipynb<br />
Clean patches are extracted from 'training_data/sub-TCRc007/ses-1/dwi' and saved in 'data/npy_data'.<br /><br />

Prospective study:<br />
$ python Generate_patches_prospective_DWI.ipynb<br />
Clean patches are extracted from 'Training_datab3000/04032021/processed' and saved in 'data/npy_data'.<br /><br />

**Train and test**<br />
$ python Retrospective_high_b_value_DWI_Denoising.ipynb<br />
$ python Prospective_high_b_value_DWI_Denoising.ipynb<br />



**Results**
