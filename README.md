# 🍼 Early Detection of Fetal Distress Using Machine Learning  

---

## 📌 Introduction  
Fetal health monitoring is crucial to detect pregnancy complications early.  
This project uses **Cardiotocography (CTG) data** and **Machine Learning** to classify fetal health as:  
- **Normal**  
- **Suspect**  
- **Pathological**  

A **Flask web application** provides real-time predictions with a user-friendly interface.  

---

## ⚡ Features  
- CTG dataset with 21 features  
- ML models: Random Forest, Logistic Regression, KNN, SVM, Gradient Boosting  
- Best Model: **Random Forest (95% Accuracy, ROC-AUC 0.97)**  
- Flask-based web app  
- Demo input support (Normal / Suspect / Pathological)  
- Probability visualization with progress bars  

---

## 🚀 Run Locally  

### 1. Clone the project
```bash
git clone https://github.com/YOUR-USERNAME/fetal-health-prediction.git
cd fetal-health-prediction
2. Create a virtual environment
bash
Copy code
# Linux / Mac
python -m venv venv
source venv/bin/activate  
```
# Windows
```bash
#linux/mac
python -m venv venv
venv\Scripts\activate
```
3. Install dependencies
```bash
pip install -r requirements.txt
```
4. Run the app
```bash
python app.py
```
5. Open in browser
```cpp
http://127.0.0.1:5000/
```
🖥️ Usage / Examples
```
Web Interface
Input CTG parameters manually

Or load demo data (Normal / Suspect / Pathological)

View prediction + probabilities instantly
```
Example Output
```json
{
  "result": "Pathological",
  "probabilities": {
    "Normal": "5.2%",
    "Suspect": "10.7%",
    "Pathological": "84.1%"
  }
}
```

## 📊 Screenshots
### ROC Curves

#### KNN Model
![image alt](https://github.com/NKuladeep/Early-Distress_of_Fetal_Distress/blob/35e9618adaebf51a5520f87d5e87b718f9df9a5e/static/images/ctg_model_comparison.png)

#### Logistic Regression
![ROC Curve - Logistic Regression](static/images/ctg_roc_curve_logistic_regression.png)

#### Random Forest
![ROC Curve - Random Forest](static/images/ctg_roc_curve_random_forest.png)

#### Alternative KNN Visualization
![ROC Curve - KNN Alt](static/images/roc_curve_knn.png)

#### Alternative Random Forest Visualization
![ROC Curve - Random Forest Alt](static/images/roc_curve_random_forest.png)

#### Multiple Models Comparison
![ROC Curve - Model Comparison](static/images/roc_curves_comparison.png)


⚙️ TECH STACK

```
    Frontend: HTML, CSS, Bootstrap
    Backend: Flask
    ML Models: scikit-learn (Random Forest, Logistic Regression, KNN, SVM, Gradient Boosting)
    Deployment: Localhost / Future: AWS, Azure, Heroku
```

🔑 ENVIRONMENTAL VARIABLES

    To run this project, you may need to set the following environment variables:
```env
   FLASK_APP = app.py
   FLASK_ENV = development
```
🧪 RUNNING TESTS

 ```bash
   pytest tests/
   #(Add test scripts in a tests/ folder.)
```

📈 OPTIMIZATIONS
```
    Applied GridSearchCV for hyperparameter tuning

   Balanced classes with class_weight=balanced

   Feature importance ranking with Random Forest
```

🛠️ ROADMAP
```
   Model training & evaluation '/n'

   Flask web app deployment

   Cloud deployment (AWS/Heroku)

  Real-time CTG data integration

 Add deep learning models (LSTMs/Neural Networks)
```

🙋 FAQ
```
Q: Can this system replace doctors?**
A: No. It is a decision-support tool, not a replacement.

Q: Which dataset is used?
A: Public CTG dataset (UCI / Kaggle).
```

👨‍💻 AUTHORS

@Nageti-Kuladeep – ML & Backend

Team Members – Data preprocessing, Model training, UI

🏅 ACKNOWLEDGMENTS

UCI Machine Learning Repository

Kaggle for dataset hosting

Journal of Engineering Sciences (Vol 16, Issue 05, 2025) for publication

📄 LICENSE

This project is licensed under the MIT License – see the LICENSE file for details.

💡 LESSONS LEARNED

Importance of handling class imbalance in medical datasets

Ensemble models (Random Forest, Gradient Boosting) perform best in healthcare ML

Usability is critical for clinical adoption

🤝 CONTRIBUTING
```
Contributions are welcome!

Fork the repo

Create a feature branch (git checkout -b feature/xyz)

Commit changes (git commit -m "Added xyz")

Push branch (git push origin feature/xyz)

Open a Pull Request
```
❤️ SUPPORT

If you found this helpful:

⭐ Star this repo

📝 TEAM OF PUBLICATION :

Uma Manasa T., Prasanthi K., Kuladeep N., et al. Early Detection of Fetal Distress Using ML Models, JES, 2025
