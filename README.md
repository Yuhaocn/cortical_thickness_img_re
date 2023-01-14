# cortical_thickness_img_recognition
The goal of this experiment is to develop an algorithm to estimate cortical thickness map from a raw T1-weighted image. In this experiment I will combine diffeomorphic registration based cortical thickness (DiReCT) measure with Advanced Normalization Tools (ANTS) and DL+DiReCT, a tool combines a deep learning-based neuroanatomy segmentation and cortex parcellation with a diffeomorphic registration technique to measure cortical thickness from T1w MRI.

![2 I51U(MF36}(573RV}%)5X](https://user-images.githubusercontent.com/102940480/212444026-b99d3ffd-fdde-4327-a596-f1f81d57b38d.png)
![Y47N@V%MW0Y_{86SP1UPQO6](https://user-images.githubusercontent.com/102940480/212444033-89518fee-74bb-44ad-a395-ea6f7ec4509b.png)
1.	Abstract
The goal of this experiment is to develop an algorithm to estimate cortical thickness map from a raw T1-weighted image. In this experiment I will combine diffeomorphic registration based cortical thickness (DiReCT) measure with Advanced Normalization Tools (ANTS) and DL+DiReCT, a tool combines a deep learning-based neuroanatomy segmentation and cortex parcellation with a diffeomorphic registration technique to measure cortical thickness from T1w MRI.
2.	Enviroment
System: Linux 4.4.0 Ubuntu 20.04.4 LTS
package used: DL+DiReCT, HD-BET, ANTsPy, nilearn
Usage
Run dl+direct on a T1-weighted MRI including skull-stripping (--bet) using HD-BET with:
source activate DL_DiReCT
dl+direct --subject <your_subj_id> --bet <path_to_t1_input.nii.gz> <output_dir>
4.	Conclusion
In this experiment I study the previous research about cortical thickness and how researchers using principled approach to find correspondence between WM and GM surfaces using shape-constrained Diffeomorphic mapping. Due to limitations of this study of brain study and working on MRI image, this experiment is based on tools created by previous researchers. In the future study, I would like to expand the current work to increase the efficiency and accuracy base on the current algorithm.
REFERENCES
[1] Das, Sandhitsu R., et al. "Registration based cortical thickness measurement." Neuroimage 45.3 (2009): 867-879.
[2] Avants, Brian B., Nick Tustison, and Gang Song. "Advanced normalization tools (ANTS)." Insight j 2.365 (2009): 1-35.
[3] Rebsamen, M, Rummel, C, Reyes, M, Wiest, R, McKinley, R.
Direct cortical thickness estimation using deep learning‐based anatomy segmentation and cortex parcellation.
Human brain mapping. 2020; 41: 4804-4814. https://doi.org/10.1002/hbm.25159
[4] Sharaff, Aakanksha, and Harshil Gupta. "Extra-tree classifier with metaheuristics approach for email classification." Advances in computer communication and computational sciences. Springer, Singapore, 2019. 189-197.

