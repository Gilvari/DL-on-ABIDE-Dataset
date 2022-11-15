# Functional-Connectivity-and-Classification-On-Autism-FMRI
Mining resting-state fMRI Signal to Develop Functional Connectivity and Classification
Install Dependency
The required dependencies to use the software are:
1.	Python >= 3.5,
2.	setuptools
3.	Numpy >= 1.11
4.	SciPy >= 0.19
5.	Scikit-learn >= 0.19
6.	Joblib >= 0.12
7.	Nibabel >= 2.0.2
8.	matplotlib >= 1.5.1
Data Fetching
You have to fetch the data using Nilearn built in function
If you want to run the tests, you need pytest >= 3.9 and pytest-cov for coverage reporting.
nilearn.datasets.fetch_abide_pcp(data_dir=None, n_subjects=None, pipeline='cpac', band_pass_filtering=False, global_signal_regression=False, derivatives=['func_preproc'], quality_checked=True, url=None, verbose=1, **kwargs)
Fetch ABIDE dataset
Fetch the Autism Brain Imaging Data Exchange (ABIDE) dataset wrt criteria that can be passed as parameter. Note that this is the preprocessed version of ABIDE provided by the preprocess connectome projects (PCP).
Parameters/Arguments
data_dir: string, optional
Path of the data directory. Used to force data storage in a specified location. Default: None
n_subjects: int, optional
The number of subjects to load. If None is given, all available subjects are used (this number depends on the preprocessing pipeline used).
pipeline: string, optional
Possible pipelines are “ccs”, “cpac”, “dparsf” and “niak”
band_pass_filtering: boolean, optional
Due to controversies in the literature, band pass filtering is optional. If true, signal is band filtered between 0.01Hz and 0.1Hz.
global_signal_regression: boolean optional
Indicates if global signal regression should be applied on the signals.
derivatives: string list, optional
Types of downloaded files. Possible values are: alff, degree_binarize, degree_weighted, dual_regression, eigenvector_binarize, eigenvector_weighted, falff, func_mask, func_mean, func_preproc, lfcd, reho, rois_aal, rois_cc200, rois_cc400, rois_dosenbach160, rois_ez, rois_ho, rois_tt, and vmhc. Please refer to the PCP site for more details.
quality_checked: boolean, optional
if true (default), restrict the list of the subjects to the one that passed quality assessment for all raters.
kwargs: parameter list, optional
Any extra keyword argument will be used to filter downloaded subjects according to the CSV phenotypic file. Some examples of filters are indicated below.
SUB_ID: list of integers in [50001, 50607], optional
Ids of the subjects to be loaded.
DX_GROUP: integer in {1, 2}, optional
1 is autism, 2 is control
DSM_IV_TR: integer in [0, 4], optional
O is control, 1 is autism, 2 is Asperger, 3 is PPD-NOS, 4 is Asperger or PPD-NOS
AGE_AT_SCAN: float in [6.47, 64], optional
Age of the subject
SEX: integer in {1, 2}, optional
1 is male, 2 is female
HANDEDNESS_CATEGORY: string in {‘R’, ‘L’, ‘Mixed’, ‘Ambi’}, optional
R = Right, L = Left, Ambi = Ambidextrous
HANDEDNESS_SCORE: integer in [-100, 100], optional
Positive = Right, Negative = Left, 0 = Ambidextrous
![image](https://user-images.githubusercontent.com/118232462/201933820-dc4dc745-b3ec-42a6-ae50-b4d85ccd57e6.png)
