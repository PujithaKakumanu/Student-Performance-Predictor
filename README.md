# **🚀 Student Performance Predictor 🚀**

## **Overview**
The **Student Performance Predictor** is a data-driven tool designed to predict a student's **SGPA** (Semester-based CGPA) with exceptional accuracy. By analyzing factors such as study hours, tutoring, absences, parental support, extracurricular activities, and sports, this project provides students with actionable insights to maximize their academic performance.

---

## **Key Features**

1. **High-Accuracy Predictions:**
   - Predicts SGPA with an impressive **98% accuracy**. 📈

2. **Visual Analysis:**
   - Generates a **pie chart** of input data for easy understanding.
   - Displays a **comparison graph** between recommended study time (minimum 15 hours) and actual study time, encouraging better time management.

3. **Personalized Feedback:**
   - Provides tailored suggestions to enhance academic performance, such as:
     - "Increase your study time to at least 12–15 hours per week for a decent SGPA."
     - "You have too many absences; please try to manage your schedule better."
     - "Consider tutoring to boost your academic performance."

---

## **Technologies Used**
- **Backend:** Flask (Python)
- **Frontend:** HTML, CSS
- **Machine Learning:** Scikit-learn (Gradient Boosting Regressor)
- **Data Visualization:** Matplotlib, Plotly
- **Model Serialization:** Joblib

---

### **2. Install Dependencies**
Before you begin, ensure that you have the Python installed:
Create a virtual environment and install the required packages:
```bash
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate      # For Windows
pip install flask pandas joblib numpy matplotlib seaborn scikit-learn
 
```

### **3. Train the Model**
Run the `train_model.py` script to train the machine learning model:
```bash
python train_model.py
```
This will create a `model.pkl` file for predictions.

### **4. Run the Application**
Start the Flask server:
```bash
python app.py
```
Access the application at `http://127.0.0.1:5000`.

---

## **How It Works**

### **Input Data**
- **Study Time:** Weekly study hours, including self-study and assignments.
- **Absences:** Number of absences for the semester.
- **Tutoring:** Whether the student receives tutoring (Yes/No).
- **Parental Support:** Level of parental involvement.
- **Extracurricular Activities & Sports:** Participation in activities outside academics.

### **Output**
- **Predicted SGPA:** The semester-based CGPA.
- **Feedback:** Tailored advice based on input factors.
- **Visualization:**
  - Pie chart of input data distribution.
  - Comparison graph of study time versus recommended hours.

---

## **Example**

### **Input:**
```json
{
  "StudyTimeWeekly": 10,
  "Absences": 8,
  "Tutoring": 0,
  "ParentalSupport": 1,
  "Extracurricular": 1,
  "Sports": 0
}
```

### **Output:**
- **Predicted SGPA:** 7.8
- **Feedback:** 
  - "Increase your study time to at least 12–15 hours per week for a decent SGPA."
  - "You have too many absences; please try to manage your schedule better."

---

## **Visualization**
- **Pie Chart:** Provides a breakdown of the input factors.
- **Graph:** Compares actual weekly study time to the recommended 15 hours.

---

## **Future Enhancements**
- Include more features for prediction, such as:
  - Time spent on specific subjects.
  - Part-time job status.
  - Sleep schedule and its impact on performance.
- Integrate a feedback tracking system to help students monitor progress over time.
- Build mobile compatibility for broader accessibility.

---
