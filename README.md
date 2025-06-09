# Predicting Ratings for Dialysis Facilities in the United States 

## creating a data science blog post | udacity-ds-project1

### Author: 
Benjamin Mardin

### Topic: 
Predicting Ratings for Dialysis Facilities in the United States 

### Motivation: 
With healthcare costs skyrocketing, it is more important than ever for patients have the information they need to make the right decision regarding their health.  Dialysis in particular is a medical service where many different providers can offer nearly identical services, so giving patients the transparency into ratings information can allow patients to choose facilities that give them the best possible health outcomes. The data from Centers for Medicare and Medicaid Services (CMS) provides potentially useful but unwieldy information regarding Dialysis facilities across the United States, but with some clean up and modeling, we can use this data to understand how the ratings work, if they are related to actual patient health outcomes, and if there are other factors besides patient health outcomes at play in a facility's rating.  Businesses that work with Dialysis facilities may also be interested in this transparency, as they either aim to improve existing facilities, open new ones, or look to work along with the current players in the Dialysis facility marketplace.

### Repository Files:
- README.md | overview of the project
- Dialysis Analysis.ipynb | jupyter notebook containing code for ingesting, analyzing, cleaning, and modeling Dialysis Facility data
- DFC_FACILITY.csv | a copy of the latest (as of 2025-06-04) 'Dialysis Facility - Listing by Facility' file from Centers for Medicare and Medicaid Services. originally sourced from: https://data.cms.gov/provider-data/dataset/provider-data/
- DF_Data_Dictionary.pdf | a copy of the latest (as of 2025-06-04) Data Dictionary for the Dialysis Facility data.  originally sourced from: https://data.cms.gov/provider-data/sites/default/files/data_dictionaries/dialysis/DF_Data_Dictionary.pdf

  
### Results Summary:
- there are over 7000 dialysis facilities across the united states
- 11 different regions included in CMS data have 0 five-star facilities
- I was able to predict a facility's rating based on its health outcomes better than a dummy regressor model
- the model I created had 0.52 R-squared, indicating a relationship between the features (health outcomes + ownership model + profit motive) and the target (rating)
- there is potential confounds because of imbalanced data, particularly around ownership structure and profit motive

### Packages:
- matplotlib == 3.5.3
- pandas == 1.3.5
- seaborn == 0.12.2
- scikit-learn == 1.0.2

### Acknowledgements:
- Udacity data scientist program | introduction to data science and supervised machine learning
- CKD and Dialysis background information sourced from :

[1] Centers for Disease Control and Prevention. Chronic Kidney Disease in the United States, 2023. Atlanta, GA: US Department of Health and Human Services, Centers for Disease Control and Prevention; 2023. https://www.cdc.gov/kidney-disease/php/data-research/index.html

[2] United States Renal Data System. 2023 USRDS Annual Data Report: Epidemiology of kidney disease in the United States. National Institutes of Health, National Institute of Diabetes and Digestive and Kidney Diseases, Bethesda, MD, 2023. https://usrds-adr.niddk.nih.gov/2023/end-stage-renal-disease/1-incidence-prevalence-patient-characteristics-and-treatment-modalities

[3] https://data.cms.gov/provider-data/dataset/23ew-n7w9#overview

[4] https://www.cms.gov/Medicare/Quality-Initiatives-Patient-Assessment-Instruments/HomeHealthQualityInits/Downloads/QoPC-Fact-Sheet-For-HHAs_UPDATES-7-24-16-2.pdf
Shout out to all the pears
