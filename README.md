# PCOS Detection using Machine learning models and XAI for clinical interpretability and Trust

### There will always be signs 
PCOS is like popcorn all over the ovary, it is a change in the anatomy of the ovary which results in hormonal changes. Having PCOS means that the power of insulin (a hormone responsible for processing carbs, sugars and some proteins) drops. This results in the body trying to produce more insulin which results in increased testosterone levels. The ovary’s environment has changed and there is a lot of testosterone in it that is not able to ovulate the eggs properly. Increased insulin levels also lead to other complications like type 2 diabetes, cardiovascular diseases, ovarian cancers and even autoimmune conditions. (American Medical Association, 2025)

![PCOS image](https://my.clevelandclinic.org/-/scassets/images/org/health/articles/8316-polycystic-ovary-syndrome-pcos) (Polycystic Ovary Syndrome (PCOS), 2025)

### What decision can this project help to make?
There are two cases. First, if features like skin darkening, hair growth, etc., (non-invasive parameters) dominate the feature importance graphs, then this application could serve as a firsthand screening process to women who want to know about their body and make a decision to visit a healthcare provider or not. (Note: again, this depends on the data quality and diversity)

If features that require medical tests like follicle number or AMH(invasive parameters), dominate the feature importance matrix, then this application could be deployed to healthcare providers, where the patients/doctor (depending upon the health care management procedures) can use this as a tool to see where they are in the spectrum. 

The best part is the explainable AI here which allows us to answer the question “What features actually contribute to predicting the PCOS?” This enables doctors to understand where to look closely and aid in better diagnosis. 
(All in all, for all this to happen, we need quality, diversified large scale patient clinical test data.) Our tool can serve as a first hand screening before the physical exam and serve as a tool in detection after the following tests have been taken by the patients. 

### Final Results:






















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
