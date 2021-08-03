# High-b-value-DWI-denoising
Deep learning based denoising can improve signal-to-noise ratio in high b-value diffusion imaging with reduced acquisition time. We applied deep learning based denoising method on retrospective and prospective high b-value DWI with b-value>=2000s/mm<sup>2</sup>.The base network architecture, we adpated from the  keras implemention of the paper [Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising](https://ieeexplore.ieee.org/abstract/document/7839189).We used unsharp masking after denoising to preserve the modest details.

**Prepare training data**<br />
_`$ python Generate_patches_for_retrospective_DWI.ipynb`_<br /><br />
The DnCNN model was trained using high b-value DWI from open neuro databse.We used 150 slices from the original image('training_data/sub-TCRc007/ses-1/dwi') to create clean patches from the above mention python file  and saved in  'data/npy_data'.Later, extrxted 219,000  noisy and clean patches for training the DnCNN model.<br /><br />.
 

**Train and test**<br />
_`$ python Retrospective_high_b_value_DWI_Denoising.ipynb`_ <br /><br />
_`$ python Prospective_high_b_value_DWI_Denoising.ipynb`_ <br /><br />


