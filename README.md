# Causal-Deep-Learning-on-Electronic-Health-Records-via-Time-Varying-Patient-Specific-Baselines
## Project Description
  Our goal is to investigate causal modeling mechanisms in deep learning from electronic health records (EHRs). Deep sequence models are achieving remarkable accuracy in medical prediction. Still, when we learn a deep sequence model to predict a future event, such as myocardial infarction (MI, or heart attack) from EHR data, often some of the most predictive variables are treatments to prevent that event or condition or reduce its severity. As a concrete example, a top predictor for MI is beta blocker prescription—has the patient been prescribed a beta blocker? Although the beta blocker prescription reduces MI risk, it predicts increased MI risk simply because it indicates the clinician already knows the patient is at risk for MI.

 

This project specifically aims to alleviate the problem above by considering time-varying patient-specific baselines as part of the predictive model. These baselines are trained alongside the parameters of the underlying neural network model, allowing for an efficient method of identifying to what extent each patient's key properties contribute to future health outcomes. The patient-specific baselines need to be regularized or constrained to limit the discrepancy between population-level and patient-level baselines, as well as the difference between each patient's baselines at consecutive points over time.

![image](https://github.com/user-attachments/assets/c7e8339b-2c7b-4cfa-8311-28b15a3ad5c5)
- Arrow means the parent will increase the risk of child. Higher baseline value (cvr) is related to high risk of MI. 
- “+++” indicating increasing the chance of occurrence, “---” indicating decreasing the chance of occurrence.
- Acid reducer is left alone currently.
