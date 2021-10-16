# 8200Bio Data Challenge
In this challenge the goal was to predict the medical specialty from the transcription field, <br/>
that is for each file (unique transcription) need to predict whether it belongs to each label (medical specialty).<br/>
You can find the data [here](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Data/data.csv).

## My strategy
* Clear the data and convert it to features.<br/>
  [The notebook is here](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Text%20cleaning%20%26%20processing%20.ipynb).
* Make the data balanced for a more realistic prediction.<br/>
  [The notebook is here](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Imbalanced%20data%20handling%20.ipynb).
* Train a model for each specialty and test it.<br/>
  [The notebook is here](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Training%20%26%20Testing.ipynb).

## Accuracy results
Specialty  | Accuracy score
------------- | -------------
Allergy / Immunology  | 96.46%
Autopsy accuracy  | 99.51%
Bariatrics accuracy  | 97.09%
Cardiovascular / Pulmonary  | 97.92%
Cosmetic / Plastic Surgery  | 96.81%
Dentistry  | 96.87%
Dermatology  | 96.99%
ENT - Otolaryngology  | 96.85%
Emergency Room Reports  | 96.67%
Endocrinology  | 96.81%
Gastroenterology  | 97.64%
General Medicine  | 96.93%
Hematology - Oncology  | 96.86%
Hospice - Palliative Care  | 97.36%
Lab Medicine - Pathology  | 96.85%
Nephrology  | 97.05%
Neurology  | 97.48%
Neurosurgery  | 96.71%
Obstetrics / Gynecology  | 97.18% 
Office Notes  | 97.12%
Ophthalmology  | 96.86%
Orthopedic  | 97.01%
Pain Management  | 96.99%
Pediatrics - Neonatal  | 96.92%
Physical Medicine - Rehab  | 96.57%
Podiatry  | 96.9%
Psychiatry / Psychology  | 96.99%
Radiology  | 97.65%
Rheumatology  | 96.82%
Sleep Medicine  | 96.64%
Surgery  | 96.71%
Urology  | 97.12%
Speciality  | 96.85%
