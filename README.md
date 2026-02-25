# in_search_of_truth
Repository for paper "In search of truth". 

This data was used for the following project: 'In search of truth: A refined approach to data collection and annotation for BERT-based misinformation detection'. For this project, we developed a codebook to classify misinformation and other content-related characteristics, such as incivility, in Tweets, and elaborately trained four student assistants to classify 3400 Tweets using this codebook. 
The paper and codebook are published in Computational Communication Research. 

This repository contains the following documents:
- Appendix.docx. The appendix includes a codebook and supplementary materials used to code the data, and results of robustness checks. 
- data. csv. Data contains Tweet ids and labels (e.g., misinformation, incivility) given by coders. The Tweet IDs correspond to Dutch-language Tweets about covid that were posted between February 2020 and February 2022. The data used for this project also contained the tweets' texts and dates. However, the published data does not include texts and dates, because this is not in line with Twitter/X's policies. See below for a schema of the original data.
- data_codebook.txt. Codebook that includes all variables in the data and a short description. See the paper for a full codebook on how the data was annotated. 
- Train_test_BERT.ipynb. Python code to run the main analyses. Pre-processes data, trains a BERT model, and runs some additional analyses.
- Robustness check suggestive misinformation.ipynb: Python code to run robustness check. Trains a BERT model with data where suggestive misinformation is included in the 'accurate information' and not th 'misinformation'category (as in the main analyses).
- Data_rob_sug.csv: Data where suggestive misinformation is included in the 'accurate information' and not the 'misinformation' category.
- Robustness check oversampling.ipynb: Python code to tun robustness check. Trains a BERT model with data where the 'accurate information' class is given more weight to represent real-world distributions of accurate information and misinformation. 

The original data contains the following variables: id,Coder.ID,Information_category,Attribution,Att_D_pol,Att_D_gov,Att_f_pol_gov,Att_mainme,Att_altme,Att_ind,Att_other,Att_no,Sentiment,Authority_ref,Incivility,Emotional,Fearmongering,Topics,Conspiracy,Gov_pol_org,Health_serv,Media,Other_nongov,Ind_com,Other,No,Scient,Misinfo_bin,label_mis, text, date (See Data_codebook.txt for an explanation of the variables)




