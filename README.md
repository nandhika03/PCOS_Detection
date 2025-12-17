# PCOS Detection using Machine learning models and XAI for clinical interpretability and Trust

### There will always be signs 
PCOS is like popcorn all over the ovary, it is a change in the anatomy of the ovary which results in hormonal changes. Having PCOS means that the power of insulin (a hormone responsible for processing carbs, sugars and some proteins) drops. This results in the body trying to produce more insulin which results in increased testosterone levels. The ovary’s environment has changed and there is a lot of testosterone in it that is not able to ovulate the eggs properly. Increased insulin levels also lead to other complications like type 2 diabetes, cardiovascular diseases, ovarian cancers and even autoimmune conditions. (American Medical Association, 2025)

![PCOS image](https://my.clevelandclinic.org/-/scassets/images/org/health/articles/8316-polycystic-ovary-syndrome-pcos) 


### What decision can this project help us to make in the Real World?
There are two cases. 
1. First, if features like skin darkening, hair growth, etc., (non-invasive parameters) dominate the feature importance graphs, then this application could serve as a firsthand screening process to women who want to know about their body and make a decision to visit a healthcare provider or not. (Note: again, this depends on the data quality and diversity)

2. If features that require medical tests like follicle number or AMH(invasive parameters), dominate the feature importance matrix, then this application could be deployed to healthcare providers, where the patients/doctor (depending upon the health care management procedures) can use this as a tool to see where they are in the spectrum. 

The best part is the explainable AI here which allows us to answer the question “What features actually contribute to predicting the PCOS?” This enables doctors to understand where to look closely and aid in better diagnosis. 
(All in all, for all this to happen, we need quality, diversified large scale patient clinical test data.) Our tool can serve as a first hand screening before the physical exam and serve as a tool in detection after the following tests have been taken by the patients. 

### Final Results:
The left follicle number, skin darkening, hair growth and weight gain were the top 4 important features from the SVM with ADASYN model achieving a 100% recall score. 
<img width="1473" height="345" alt="Screenshot 2025-12-16 090501" src="https://github.com/user-attachments/assets/b71e43bd-8c6d-409f-a2a1-7b25dfd39fb0" />
Recall was chosen, as false negatives would be costly in this case. Model was examined for overfitting and XAI methods were further used to verify reliability of feature importance here

### Limitations:
However further study on methods and order of pre-processing steps is required to be clinically relevant, which will be Part II of this project, the workflow has already been designed and only testing of the models is left. 
Can be deployed as a first hand screening tool on cloud streamlit or healthcare facilities.

### Part II of the PCOS Detection & Raw FlowChart of clean thought-through pipeline:
This time, I do not claim to do it the perfect way, but I believe it could be a step in the right direction. I do not want to overclean my data or dismiss important medical information as anomalies. The rough report of th part II can be found [here]([url](https://docs.google.com/document/d/1n2fAzg-CMG7fx4GpJBu5E0ngXmNPi4VS9ETC5Uwic80/edit?tab=t.d0a5tre5drgk))

<img width="1920" height="1080" alt="PCOS_ProjectFlowchart" src="https://github.com/user-attachments/assets/820c78fc-1a59-4779-89b8-e3e292927eed" />

### [Dataset:](https://www.kaggle.com/datasets/prasoonkottarathil/polycystic-ovary-syndrome-pcos/data)
Source of data: The dataset we used for this project had been obtained from kaggle. Prasoon kottarathil, owner of the data, claims to have collected this data from 10 different hospitals across Kerala, India. In another comment, he also reassures that there are no ethical concerns in using the data for academic purposes and that the patient anonymity has been maintained. Both raw and cleaned datasets are available in this repository's dataset folder.

### Main Challange I faced with this data:
Data quality issues and then the main thing is that there is nobody to enquire and validate the data, especially the outliers, because in medical data, outliers can be important.

#### Environment set up:
#### Creating venv:

conda create --name pcosvenv python=3.10

#### Activation of venv:

conda activate pcosvenv

#### Git commangds:

git init
git add README.md

#### create a repo in github as well

git commit -m "readme file"
git status
git branch -M main
git status
git remote add origin https://github.com/nandhika03/PCOS_Detection.git
git remote -v
git remote add origin https://github.com/nandhika03/PCOS_Detection.git
git push -u origin main
git pull
