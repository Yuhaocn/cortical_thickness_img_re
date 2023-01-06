OS: linux
steps:
Download and install Miniconda and create a new conda environment:
	conda create -y -n DL_DiReCT python=3.7
	source activate DL_DiReCT
Install DL+DiReCT
	git clone https://github.com/SCAN-NRAD/DL-DiReCT.git
	cd DL-DiReCT
	pip install -e .
Run dl+direct on a T1-weighted MRI including skull-stripping (--bet) using HD-BET with:
	source activate DL_DiReCT
	dl+direct --subject <your_subj_id> --bet <path_to_t1_input.nii.gz> <output_dir>
Following files of interest are generated in the output directory:

- T1w_norm.nii.gz		Re-sampled input volume
- T1w_norm_seg.nii.gz		Segmentation
- T1w_norm_thickmap.nii.gz	Thickness map
- result-vol.csv		Segmentation volumes
- result-thick.csv		ROI-wise mean cortical thickness
- result-thickstd.csv		ROI-wise standard deviations of cortical thickness
- label_def.csv			Label definitions of the segmentation

[1]Rebsamen, M, Rummel, C, Reyes, M, Wiest, R, McKinley, R.
Direct cortical thickness estimation using deep learning‐based anatomy segmentation and cortex parcellation.
Human brain mapping. 2020; 41: 4804-4814. https://doi.org/10.1002/hbm.25159