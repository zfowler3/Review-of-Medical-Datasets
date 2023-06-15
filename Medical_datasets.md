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
+ [Additional info](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community)

## [PadCHEST](https://arxiv.org/abs/1901.07441)
+ Type: chest x-ray image dataset
