# NI Scratch Detection (Machine Learning Project)

This project solves a real-world problem in the semiconductor industry — detecting scratches on silicon wafers by analyzing logical wafer maps.

### 📌 Task Summary

Given the positions (`DieX`, `DieY`) and status of individual dies on wafers, predict whether a die is part of a scratch (including `Scratch` and `Ink`).

### 🧠 Model

- Algorithm: Random Forest Classifier
- Features used: `DieX`, `DieY`, `IsGoodDie`
- Handled severe class imbalance using `class_weight='balanced'`
- Applied business constraint: filtered wafers with yield < 0.6

### 📊 Results


- Achieved **84% recall** on Scratch class
- Predicted scratches on **5.68%** of test dies
- Visual validation confirms alignment of predicted scratch clusters

### 📦 Files

- `scratch_detection_assignment.ipynb` — notebook with full workflow
- `submission.csv` — test predictions (WaferName, DieX, DieY, IsScratchDie)
- `images/` — wafer map visualizations

### 💡 Future Work

- CNN-based scratch detection on 2D wafer grid images
- Graph-based models (GNN) to model die adjacency
- API deployment using FastAPI or Flask

---

👤 **Author**: Nikita Marshchonok  
📧 n.marshchonok@gmail.com  
🔗 [LinkedIn](http://www.linkedin.com/in/nikita-marshchonok) | [GitHub](https://github.com/NikitaMarshchonok)
