# Multiple Disease Prediction System

A comprehensive machine learning-based system for predicting multiple diseases including Diabetes, Heart Disease, and Parkinson's Disease using various clinical and diagnostic parameters.

## 🩺 Overview

This system utilizes machine learning algorithms to predict the likelihood of three major diseases based on relevant medical parameters. The system is designed to assist healthcare professionals in early diagnosis and risk assessment.

## 🔍 Supported Diseases

### 1. Diabetes Prediction
### 2. Heart Disease Prediction  
### 3. Parkinson's Disease Prediction

---

## 📊 Disease Information & Parameters


### 1. Diabetes Mellitus

**Description:**
Diabetes is a group of metabolic disorders characterized by high blood sugar levels over a prolonged period. Type 2 diabetes, the most common form, occurs when the body becomes resistant to insulin or doesn't produce enough insulin. Early detection is crucial for preventing complications such as cardiovascular disease, kidney damage, and nerve damage.

**Risk Factors:**
- Family history and genetics
- Obesity and physical inactivity
- Age (risk increases with age)
- Gestational diabetes history
- High blood pressure and cholesterol

![Diabetes](https://raw.githubusercontent.com/MunishUpadhyay/Material/refs/heads/main/Screenshot%202025-07-18%20224903.png)

**Parameters Used:**
- **Pregnancies**: Number of times pregnant (0-17)
- **Glucose**: Plasma glucose concentration after 2-hour oral glucose tolerance test (mg/dL)
- **BloodPressure**: Diastolic blood pressure (mm Hg)
- **SkinThickness**: Triceps skin fold thickness (mm)
- **Insulin**: 2-Hour serum insulin (mu U/ml)
- **BMI**: Body Mass Index (weight in kg/(height in m)²)
- **DiabetesPedigreeFunction**: Diabetes pedigree function (genetic predisposition score)
- **Age**: Age in years

---

### 2. Heart Disease

**Description:**
Heart disease refers to several types of heart conditions, with coronary artery disease being the most common type. It occurs when the arteries that supply blood to the heart muscle become hardened and narrowed due to cholesterol and other material buildup (plaque) on their inner walls. This condition can lead to heart attacks, chest pain, and other serious complications.

**Risk Factors:**
- High blood pressure and cholesterol
- Smoking and diabetes
- Family history of heart disease
- Age and gender
- Obesity and physical inactivity
- Stress and poor diet

![Heart](https://raw.githubusercontent.com/MunishUpadhyay/Material/refs/heads/main/Screenshot%202025-07-18%20224939.png)

**Parameters Used:**
- **age**: Age in years
- **sex**: Gender (1 = male, 0 = female)
- **cp**: Chest pain type (0-3)
  - 0: Typical angina
  - 1: Atypical angina
  - 2: Non-anginal pain
  - 3: Asymptomatic
- **trestbps**: Resting blood pressure (mm Hg)
- **chol**: Serum cholesterol (mg/dl)
- **fbs**: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- **restecg**: Resting electrocardiographic results (0-2)
  - 0: Normal
  - 1: ST-T wave abnormality
  - 2: Left ventricular hypertrophy
- **thalach**: Maximum heart rate achieved
- **exang**: Exercise induced angina (1 = yes, 0 = no)
- **oldpeak**: ST depression induced by exercise relative to rest
- **slope**: Slope of the peak exercise ST segment (0-2)
- **ca**: Number of major vessels colored by fluoroscopy (0-3)
- **thal**: Thalassemia (1 = normal, 2 = fixed defect, 3 = reversible defect)

---

### 3. Parkinson's Disease

**Description:**
Parkinson's disease is a progressive nervous system disorder that affects movement. It develops gradually, often starting with a barely noticeable tremor in just one hand. The disorder also commonly causes stiffness or slowing of movement. As the disease progresses, people may have difficulty walking and talking. The disease occurs when nerve cells in the brain that produce dopamine become impaired or die.

**Risk Factors:**
- Age (most common after 60)
- Gender (men more likely than women)
- Genetics and family history
- Environmental toxin exposure
- Head trauma

![Parkinsons](https://raw.githubusercontent.com/MunishUpadhyay/Material/refs/heads/main/Screenshot%202025-07-18%20225003.png)

**Parameters Used (Voice Analysis Features):**
- **MDVP:Fo(Hz)**: Average vocal fundamental frequency
- **MDVP:Fhi(Hz)**: Maximum vocal fundamental frequency
- **MDVP:Flo(Hz)**: Minimum vocal fundamental frequency
- **MDVP:Jitter(%)**: Variation in fundamental frequency (percentage)
- **MDVP:Jitter(Abs)**: Absolute jitter in fundamental frequency
- **MDVP:RAP**: Relative amplitude perturbation
- **MDVP:PPQ**: Period perturbation quotient
- **Jitter:DDP**: Average absolute difference of differences between cycles
- **MDVP:Shimmer**: Variation in amplitude
- **MDVP:Shimmer(dB)**: Variation in amplitude (decibels)
- **Shimmer:APQ3**: Amplitude perturbation quotient (3-period)
- **Shimmer:APQ5**: Amplitude perturbation quotient (5-period)
- **MDVP:APQ**: Amplitude perturbation quotient
- **Shimmer:DDA**: Average absolute differences between amplitudes
- **NHR**: Noise-to-harmonics ratio
- **HNR**: Harmonics-to-noise ratio
- **RPDE**: Recurrence period density entropy
- **DFA**: Detrended fluctuation analysis
- **spread1**: Nonlinear measure of fundamental frequency variation
- **spread2**: Nonlinear measure of fundamental frequency variation
- **D2**: Correlation dimension
- **PPE**: Pitch period entropy

---

## 🚀 Installation

```bash
# Clone the repository
git clone https://github.com/MunishUpadhyay/multiple-disease-prediction.git
cd multiple-disease-prediction

# Install required packages
pip install -r requirements.txt
```

## 📋 Requirements

```
numpy
pandas
scikit-learn
matplotlib
seaborn
streamlit
pickle
```


## 🔧 Model Training

The system uses various machine learning algorithms including:
- Support Vector Machine (SVM)
- Logistic Regression

## 📈 Performance Metrics

- **Accuracy**: Overall prediction accuracy
- **Precision**: True positive rate
- **Recall**: Sensitivity measure
- **F1-Score**: Harmonic mean of precision and recall
- **ROC-AUC**: Area under the ROC curve

## ⚠️ Important Notes

1. **Medical Disclaimer**: This system is for educational and research purposes only. It should not be used as a substitute for professional medical advice, diagnosis, or treatment.

2. **Data Quality**: Ensure input parameters are within normal physiological ranges for accurate predictions.

3. **Model Limitations**: The predictions are based on training data and may not account for all individual variations.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- Your Name - [munishupadhyay183@.com]
- Contributors welcome!

## 🙏 Acknowledgments

- Healthcare professionals for domain expertise
- Open-source datasets used for training
- Machine learning community for algorithms and techniques

## 📞 Contact

For questions or support, please contact:
- Email: your.email@example.com
- GitHub: [MunishUpadhyay](https://github.com/MunishUpadhyay)

---

**Remember**: Always consult with healthcare professionals for medical decisions. This tool is designed to assist, not replace, medical expertise.