# graduation-project
GluCare is a web-based intelligent healthcare platform that predicts an individual’s risk of diabetes based on demographic and health-related inputs.

The system integrates:

- Machine Learning (LightGBM) for prediction
- Explainable AI (SHAP) for interpretation
- PHP backend with REST APIs
- MySQL database for data storage
- AI chatbot for user interaction

The goal of GluCare is to provide early diabetes risk detection in an accessible and understandable way.

Problem Statement

Diabetes is often diagnosed at late stages due to lack of accessible early screening tools. Traditional methods can be time-consuming and require medical supervision.

GluCare addresses this issue by providing:
- Fast online risk prediction
- Easy self-assessment
- Explainable AI results to build trust and understanding

 Features
-  Diabetes risk prediction using LightGBM
-  Explainable AI using SHAP values
-  Web-based interface
-  User authentication (login/register)
-  Chatbot integration via API
-  RESTful API backend (PHP)
-  MySQL database integration
-  Arabic language support

  Tech Stack
-  Machine Learning: LightGBM
-  Explainability: SHAP
-  Backend: PHP
-  Database: MySQL
-  APIs: REST API
-  Chatbot: External AI API
-  Frontend: HTML / CSS / JS
  
  System Workflow
1. User logs into the system
2. User enters health & demographic data
3. PHP backend sends data to ML model API
4. LightGBM model generates prediction
5. SHAP explains the prediction results
6. Output is returned to the user
7. Chatbot provides additional assistance

 Input Features
-  Age
-  Gender
-  Weight
-  Height
-  Smoking status
-  Blood pressure
-  Psychological condition
-  General health status
-  Heart condition
-  Kidney condition

Output
- Probability score (% risk)

 Explainable AI (SHAP)
SHAP is used to interpret model predictions by:
- Showing feature importance
- Explaining how each factor affects the result
- Increasing transparency and trust in AI decisions
   
Demo
A short demonstration of the system
👉 Watch the demo here:
https://drive.google.com/file/d/1Hejo2EVWCQGlozncUW3Pe-7lc93BPu5W/view?usp=drive_link


 Future Improvements
- Mobile application (Android/iOS)
- Real-time glucose monitoring integration
- Advanced deep learning models
- PDF medical report generation
- Wearable device integration



