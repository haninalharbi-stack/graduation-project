# GluCare 🩺✨
**An Intelligent Web-Based Healthcare Platform for Early Diabetes Risk Prediction & Interpretation**

[![Demo Video](https://img.shields.io/badge/🎥%20Watch-Project%20Demo-red?style=for-the-badge)](https://drive.google.com/file/d/1Hejo2EVWCQGlozncUW3Pe-7lc93BPu5W/view?usp=drive_link)

---

## 📌 Overview
**GluCare** is a web-based intelligent healthcare platform that predicts an individual’s risk of diabetes based on demographic and health-related inputs. The goal of GluCare is to provide early diabetes risk detection in an accessible and understandable way.

---

## ‼️ Problem Statement
Diabetes is often diagnosed at late stages due to lack of accessible early screening tools. Traditional methods can be time-consuming and require medical supervision. 

GluCare addresses this issue by providing:
- Fast online risk prediction.
- Easy self-assessment.
- Explainable AI results to build trust and understanding.

---

## 🚀 Key Features
- **Diabetes Risk Prediction:** Utilizing optimized LightGBM models.
- **Explainable AI (XAI):** Interpreting results via SHAP values for full transparency.
- **Web-Based Interface:** Responsive and supports Arabic language seamlessly.
- **User Authentication:** Secure login and registration systems.
- **Smart Assistance:** Chatbot integration via external AI API.
- **Robust Architecture:** RESTful API backend driven by PHP and MySQL database.

---

## 🛠️ Tech Stack
| Component | Technology Used |
| :--- | :--- |
| **Machine Learning** | LightGBM |
| **Explainability (XAI)** | SHAP |
| **Backend & APIs** | PHP (REST API) |
| **Database** | MySQL |
| **Frontend** | HTML, CSS, JavaScript |
| **Chatbot** | External AI API |

---

## 🔄 System Workflow
1. User logs into the system.
2. User enters health & demographic data.
3. PHP backend sends data to ML model API.
4. LightGBM model generates prediction.
5. SHAP explains the prediction results.
6. Output is returned to the user.
7. Chatbot provides additional assistance.

---
## 📋 Input & Output Features
### **Input Features Analyzed:**
* 👤 **Demographics:** Age, Gender
* ⚖️ **Physical Metrics:** Weight, Height
* 🫀 **Medical History:** Blood pressure, Heart condition, Kidney condition
* 🚬 **Lifestyle & Mental:** Smoking status, Psychological condition, General health status

### **✨ System Output:**
* **Probability score (% risk)** with visual SHAP feature importance to show how each factor affected the final result.

---

## 📸 User Interface Preview
Landing Page:

<img width="1403" height="690" alt="homepage" src="https://github.com/user-attachments/assets/4f6c0acf-f2b2-4a7e-86fa-98018b8d0f88" />

Profile Page: 

<img width="1403" height="698" alt="profilePage" src="https://github.com/user-attachments/assets/dde31e46-53fe-4b1f-9ed6-92ce04ad53db" />

Prediction Result:

<img width="1410" height="697" alt="prediction" src="https://github.com/user-attachments/assets/0c5c098e-0b19-4652-897a-26a51084fee5" />

Chatbot Page:

<img width="1395" height="698" alt="chatbot" src="https://github.com/user-attachments/assets/157f21f5-3a97-4879-966f-d0ea55c8179c" />


---

## 🪄 Future Improvements
- [ ] Mobile application (Android/iOS) development.
- [ ] Real-time glucose monitoring integration.
- [ ] Advanced deep learning models experimentation.
- [ ] Automated PDF medical report generation.
- [ ] Wearable device integration.

## 📊 Model Inference & Interpretation (Preview)
Here is a conceptual look at how the core Machine Learning and XAI logic runs:

```python
import lightgbm as lgb
import shap

# 1. Prediction using LightGBM
model = lgb.Booster(model_file='glucare_model.txt')
probability_score = model.predict(X_user_inputs)

# 2. Interpretation using SHAP
explainer = shap.TreeExplainer(model)
shap_values = explainer(X_user_inputs)




