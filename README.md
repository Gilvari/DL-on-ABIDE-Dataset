# DL-on-ABIDE-Dataset

#### What is autism:
Autism spectrum disorder (ASD) is a developmental disorder that affects communication and behavior. Although autism can be diagnosed at any age, it is said to be a “developmental disorder” because symptoms generally appear in the first two years of life. 
Autism is known as a “spectrum” disorder because there is wide variation in the type and severity of symptoms people experience. ASD occurs in all ethnic, racial, and economic groups. Although ASD can be a lifelong disorder, treatments and services can improve a person’s symptoms and ability to function. The American Academy of Pediatrics recommends that all children be screened for autism. 
People with ASD have difficulty with social communication and interaction, restricted interests, and repetitive behaviors. 
Doctors diagnose ASD by looking at a person’s behavior and development. ASD can usually be reliably diagnosed by the age of two. It is important for those with concerns to seek out assessment as soon as possible so that a diagnosis can be made, and treatment can begin.  
https://www.nimh.nih.gov/health/topics/autism-spectrum-disorders-asd/index.shtml


#### What is fMRI data:
An fMRI scan is a functional magnetic resonance imaging scan that measures and maps the brain’s activity. An fMRI scan uses the same technology as an MRI scan. An MRI is a noninvasive test that uses a strong magnetic field and radio waves to create an image of the brain. The image an MRI scan produces is just of organs/tissue, but an fMRI will produce an image showing the blood flow in the brain. By showing the blood flow it will display which parts of the brain are being stimulated. <br>
https://www.jameco.com/Jameco/workshop/HowItWorks/what-is-an-fmri-scan-and-how-does-it-work.html



# What is CNN-Model:
### Data description:
* The sample 3D fMRI volume series data were acquired during the four sensorimotor tasks including left-hand clenching (LH), right-hand clenching (RH), auditory attention (AD), and visual stimulus (VS) tasks [1].
* Our sensorimotor dataset includes the data from 12 subjects, each subject performed each of the four tasks (three blocks per task; 20s per block). Thus, there were 30 3D fMRI volumes for each task per subject, 120 3D fMRI volumes across all four tasks per subject, and a total of 1440 3D fMRI volumes across all subjects.


### Running code: 
* Run the ‘3dcnn_fmri_demo.ipynb’ to train a 3D-CNN model using our sample data
* Changes such as adding/removing convolution and/or pooling layers can be easily done by tweaking the 3D-CNN network structure defined in this ipython notebook code.

### Visualization of a trained 3D-CNN:
* Run the file 'saliency_map_basic.ipynb' for class saliency map visualization [2]
* Run the file 'receptive_field.ipynb' for effective receptive field visualization [3]


### References
[1] Jang, H., Plis, S.M., Calhoun, V.D. and Lee, J.H., 2017. Task-specific feature extraction and classification of fMRI volumes using a deep neural network initialized with a deep belief network: Evaluation using sensorimotor tasks. Neuroimage, 145, pp.314-328.
[2] Simonyan, K., Vedaldi, A., Zisserman, A., 2013. Deep inside convolutional networks: Visualising image classification models and saliency maps. arXiv preprint arXiv:1312.6034.
[3] Luo, W., Li, Y., Urtasun, R., Zemel, R., 2016. Understanding the effective receptive field in deep convolutional neural networks, in: Advances in Neural Information Processing Systems. pp. 4898–4906.
