# IBM Cloud

This repository contains:

1. [**Final Project → Power System Fault Detection Using Machine Learning on IBM Cloud](/Ibm-Cloud_Project/Project_Final.pdf)**  
2. [**Jupyter Notebook(Power_System_ML_Project.ipnyb)**] (/Ibm-Cloud-Project/Power_System_ML_Project.ipnyb)
3. **Introduction to RAG Lab**  
   Located in [`recipes/RAG`](recipes/RAG) and includes:
   - **LAB 1:** *RAG_with_Langchain.ipnyb*
   - **LAB 2:** *Granite_Docling_RAG.ipnyb*
  




*Project Description:*


# Problem Statement:-   
Design a machine learning model to detect and classify different types 
of faults in a power distribution system. Using electrical measurement data (e.g., 
voltage and current phasors), the model should be able to distinguish between 
normal operating conditions and various fault conditions (such as line-to-ground, 
line-to-line, or three-phase faults). The objective is to enable rapid and accurate fault 
identification, which is crucial for maintaining power grid stability and reliability. 

# Proposed Solution:-
The system addresses the challenge of fault classification in power distribution using machine learning.  
Key components include:    

Data Collection: Voltage and current phasors under normal and fault conditions from substations or simulations.  

Preprocessing: Data cleaning and feature engineering.  

ML Model: Classification model (e.g., Random Forest) trained on electrical parameters and external factors like weather.  

Deployment: Hosted on IBM Cloud Lite, using Watson Studio and Watson Machine Learning.  

Evaluation: Accuracy, Precision, Recall, F1-Score metrics.  



# Requirements
IBM Cloud account with access to Watson Studio and AutoAI
Web browser & internet
CSV dataset of electrical parameters

# Libraries Used
autoai-libs==2.0.0  

lale==0.8.0  

pandas  

numpy  

scikit-learn  


# Algorithm & Deployment
  Algorithm Selection:- Random Forest Classifier selected via IBM AutoAI for its superior accuracy and multi-class classification capabilities.
  Input Features :- Fault ID, Fault Location, Voltage, Current, Power Load, Temperature, Wind Speed, Weather, Maintenance, Component Health, Fault Duration, Downtime.
  Training Process:- 
      Utilized IBM Watson AutoAI to automate:
          Preprocessing
          Feature selection
          Hyperparameter tuning
          Model evaluation
# Deployment
      Model deployed on IBM Watson Machine Learning
      User inputs fault data via a custom UI on IBM Cloud
      Model returns fault classification in real-time

# Conclusion
      The solution successfully classifies faults like line breakage, overheating, and transformer failure using real-time data.
      Achieved high accuracy using IBM Cloud AutoAI and streamlined deployment.
      Real-world testing confirmed model reliability.
      Challenges: Model selection, deployment configuration, testing in IBM Cloud.

# References
      
- [IBM Cloud](https://cloud.ibm.com)
- [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio)
