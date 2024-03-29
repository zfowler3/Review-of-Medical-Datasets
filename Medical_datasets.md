# Review of Medical Image Datasets for Machine Learning
Brief overview of medical image datasets for machine learning, divided based off of the type of images present.

# _Chest X-ray Datasets_
## [CheXpert](https://arxiv.org/abs/1901.07031)
+ Type: chest x-ray image dataset; data collected from in-patient and out-patient centers of a hospital (USA)
+ Extracted labels: authors develop algorithm to assign chest x-ray images to 14 observations (11 of which are pathologies like pneumonia, the remaining include 'no finding', 'support devices', ...)
+ EMR data: patient sex, age, whether image is frontal/lateral, whether image is AP/PA
+ **Presence of an uncertain label:** From the authors: 'Note that the “’uncertain’ label can capture both the uncertainty of a radiologist in the diagnosis as well as ambiguity inherent in the report (“heart size is stable”).' 
+ [Additional info](https://arxiv.org/pdf/2105.03020.pdf)

## [NIH Chest X-ray 14](https://openaccess.thecvf.com/content_cvpr_2017/papers/Wang_ChestX-ray8_Hospital-Scale_Chest_CVPR_2017_paper.pdf)
+ Original dataset was Chest X-ray 8; modified to 14 to account for more disease labels
+ Type: chest x-ray image dataset; data collected from in-patient visits
+ Each image can have multi-labels; uses text mining similar to CheXpert to label images
+ Eliminates uncertain labels, unlike CheXpert
+ EMR data provides patient visit number, which is not commonly present in most medical datasets
+ Extremely easy to access
+ [Additional info](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community)

## [PadCHEST](https://arxiv.org/abs/1901.07441)
+ Type: chest x-ray image dataset with 19 differential diagnoses
+ Contains radiographic reports in Spanish
+ Contains images that have been manually labeled by experts, as well as images that were labeled in a supervised learning fashion
+ Image data can have multi-labels
+ Other provided data: StudyDate, PatientSex, ViewPosition, Modality, Manufacturer, PhotometricInterpretation, PixelRepresentation, Data representation of the pixel samples, PixelAspectRatio, SpatialResolution, BitsStored, WindowCenter, WindowWidth, Rows, Columns, XRayTubeCurrent, X-ray Tube Current, ExposureTime, Duration of x-ray exposure, Exposure, ExposureInuAs, RelativeXRayExposure
+ Provides localization information

## [JSRT Database](http://db.jsrt.or.jp/eng.php)
+ Type: chest x-ray image dataset from Japan
+ Provided data includes: patient age, gender, diagnosis (malignant or benign), X and Y coordinates of nodule, simple diagram of nodule location.
+ Lung nodule images were classified into _five groups_.
+ Need username and password to download the dataset.

## [MIMIC-CXR Database](https://physionet.org/content/mimic-cxr/2.0.0/)
+ Type: chest radiograph images
+ Contains structured labels obtained from radiology reports
+ Uses strategy from CheXpert to obtain these labels
+ Has [github repository](https://github.com/MIT-LCP/mimic-cxr) for collaborative code development

# _OCT and Fundus Datasets_

## [OLIVES Dataset](https://arxiv.org/abs/2209.11195)
+ Type: OCT and fundus image dataset (USA)
+ Dataset comprised of two clinical trials
+ Contains eyes that have Diabetic Macular Edema (DME) and Diabetic Retinopathy (DR)
+ Contains biomarkers, clinical labels (BCVA, CST), patient visit number, patient ID, and more
+ Has [github repository](https://github.com/olivesgatech/OLIVES_Dataset) for all results demonstrated in paper

## [IDRID](https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid)
+ Type: fundus dataset (India)
+ Provides information on the disease severity of DR and DME for each image
+ Website claims it is "the only dataset constituting typical diabetic retinopathy lesions and also normal retinal structures annotated at a pixel level"

## [MESSIDOR](https://www.adcis.net/en/third-party/messidor/)
+ Type: fundus image dataset collected from 3 different geographical locations
+ Contains eyes that have Diabetic Retinopathy / Diabetic Macular Edema
+ Provides severity score
+ Have to request access to dataset
+ Messidor-2 fundus images available [here](https://www.kaggle.com/datasets/mariaherrerot/messidor2preprocess); free to download and preprocessed

## [Kermany](https://data.mendeley.com/datasets/rscbjbr9sj/3)
+ Type: OCT image dataset
+ OCT images are classified as having: CNV, DME, DRUSEN, and NORMAL
+ Pre-defined train/test split
+ Also contains chest xray images

# _MRI Datasets_

## [ABIDE I & II](http://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html)
+ ABIDE I can be downloaded in a pre-processed version
+ Register online to view dataset (username+password); easy to access from the ABIDE page
+ Can download data separated based off of which site it was collected at
+ Glancing through the dataset: ABIDE II NYU has mostly data from one session; same for Caltech ABIDE I

## [ADHD-200](http://fcon_1000.projects.nitrc.org/indi/adhd200/)
+ Register online to view dataset

## [BraTS2020](https://www.med.upenn.edu/cbica/brats2020/data.html)
+ Need to request data
+ Data is accompanied with tumor annotations
+ Multi-institutional; NIfTI format

## [COBRE]

## [ADNI](https://adni.loni.usc.edu/)
+ Need to request data
+ Access to lots of other clinical information besides MRI data
+ Access to participant's data across multiple visits

## [OASIS]

# _Other Large Datasets_

## [UK Biobank](https://www.ukbiobank.ac.uk/enable-your-research/about-our-data)
+ Contains brain, heart, MRI imaging, OCT imaging, and more
+ Has repeat scanning for some patients years later (usually every 2-3 years)
+ *Pay to access the data*

## [MedMNIST](https://www.ukbiobank.ac.uk/enable-your-research/about-our-data](https://zenodo.org/records/10519652))
+ Contains 2D and 3D data from various biomedical settings, including chest x-ray, fundus, OCT, blood cells, etc.
