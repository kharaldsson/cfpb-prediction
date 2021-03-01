# cfpb-prediction
 A project to predict the outcome of CFPB complaints from the Spring of 2019.

The Consumer Financial Protection Bureau (CFPB) allows consumers to submit complaints about financial products and services. The CFPB then sends these complaints to the associated companies, who are obliged to respond within 15 days. Companies must provide consumers with a response. Between January 2015 and January 2019, just over 5% of these responses entailed monetary relief for the consumer. Many complainants choose to allow the CFPB to publish the narrative text they used to describe the issue in their own words. The CFPB posts many (but not all) of the details of these complaints online in the CFPB Consumer Complaint Database (the “Complaint Database”).

This repository includes the data and code used in an effort to use the text of consumer complaint narratives to predict whether consumers will receive monetary relif. This repository includes a tuned random forest model, which uses as predictors only discrete data readily available in the Complaint Database. It also includes a bag-of-words SVM classifier, which uses only the textual attributes of the complaint narrative.

**SVM BOW Classifier:** https://github.com/kharaldsson/cfpb-prediction/blob/main/notebooks/cfpb_SVM.ipynb

**Random Forest Classifier:** https://github.com/kharaldsson/cfpb-prediction/blob/main/notebooks/cfpb_rf.ipynb

You can find the source data for this project here: https://www.kaggle.com/kharaldsson/consumter-complaints?select=Consumer_Complaints_20190324.csv

You can find a csv version of the preprocessed data here: https://www.kaggle.com/kharaldsson/cfpb-feature-engineering/output?select=narr_df_02.csv

Otherwise, both the raw data and the preprocessed data are stored as compressed pkl files in this repository.
