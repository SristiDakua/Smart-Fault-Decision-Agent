# 🔧 Smart Fault Decision Agent – "When to Repair, Replace or Alert?"

This project is a Machine Learning prototype developed for **Xempla**'s Decision Intelligence R&D internship. It simulates how intelligent agents can support fault classification and action recommendations in real-world systems like HVAC, manufacturing equipment, or smart buildings.

---

## 🚀 Problem Statement

**"When should a system be Repaired, Replaced, Alerted, or Ignored?"**  
Using sensor inputs like temperature, vibration, pressure, and runtime hours, this agent learns to classify system health status and recommend the next action.

---

## 🧠 Model Overview

- **Input Features:**  
  - `temperature`
  - `vibration`
  - `pressure`
  - `runtime_hours`

- **Output Labels (Actions):**  
  - `0 = NO_ACTION`  
  - `1 = REPAIR`  
  - `2 = REPLACE`  
  - `3 = ALERT`

- **Model Used:** Random Forest Classifier  
- **Accuracy:** ~99% on synthetic validation data  
- **Libraries:** `scikit-learn`, `pandas`, `matplotlib`, `joblib`

---

## 📊 Sample Prediction

```python
Input Sample:
{
    'temperature': 95,
    'vibration': 8.5,
    'pressure': 25,
    'runtime_hours': 600
}

Predicted Action: REPAIR
