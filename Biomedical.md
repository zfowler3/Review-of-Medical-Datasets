# Review of Medical Datasets for Machine Learning

## [CheXpert](https://arxiv.org/abs/1901.07031)
+ Type: image dataset; data collected from in-patient and out-patient centers of a hospital (USA)
+ Extracted labels: authors develop algorithm to assign chest x-ray images to 14 observations (11 of which are pathologies like pneumonia, the remaining include 'no finding', 'support devices', ...)
+ EMR data: patient sex, age, whether image is frontal/lateral, whether image is AP/PA
+ **Presence of an uncertain label:** From the authors: 'Note that the “’uncertain’ label can capture both the uncertainty of a radiologist in the diagnosis as well as ambiguity inherent in the report (“heart size is stable”).' 
+ [Additional info](https://arxiv.org/pdf/2105.03020.pdf)

## [NIH Chest X-ray 14]()
+ Type: image dataset; data collected from in-patient visits
+ EMR data provides patient visit number, which is not commonly present in most medical datasets
