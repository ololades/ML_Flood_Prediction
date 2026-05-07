#  Hochwasser-Vorhersage mit Machine Learning

Machine-Learning-Projekt zur Vorhersage von Hochwasserrisiken mit Umwelt- und Geodaten.

Dieses Projekt vergleicht verschiedene Machine-Learning-Modelle für die Hochwasser-Vorhersage und bewertet ihre Leistung mit Klassifikationsmetriken und ROC-Analyse.

---

##  Projektübersicht

Dieses Projekt benutzt Geodaten und Umweltdaten, um gefährdete und nicht gefährdete Hochwassergebiete vorherzusagen.

Der Arbeitsprozess enthält:

- Datenvorverarbeitung
- Korrelationsanalyse
- Multikollinearitätsanalyse
- Datennormalisierung
- Modelltraining
- Hyperparameter-Optimierung
- Modellbewertung
- Speichern der Modelle für Deployment

Das Projekt vergleicht folgende Modelle:

- Random-Forest-Klassifikator
- AdaBoost-Klassifikator
- XGBoost-Klassifikator

Das beste Modell wurde gespeichert und später für die Webanwendung benutzt.

---

##  Verwendete Technologien

- Python
- GeoPandas
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Seaborn
- Matplotlib
- Joblib

---

##  Datensatz

Der Datensatz enthält Umwelt- und Geofaktoren zum Thema Hochwasser.

Beispielmerkmale:

- Elevation
- Rainfall
- Soil Type
- Land Use
- Population Density

Zielwerte:

- `0` → Kein Hochwasser
- `1` → Hochwasser

---

##  Datenanalyse

### Verteilung des Datensatzes

Der Datensatz enthält Hochwasser- und Nicht-Hochwasser-Beispiele.

![Dataset Distribution](assets/dataset_distribution.png)

---

### Korrelations-Heatmap

Pearson-Korrelationsanalyse zwischen den Merkmalen.

![Correlation Heatmap](assets/correlation_heatmap.png)

---

### VIF- und Toleranzanalyse

Multikollinearitätsanalyse mit VIF- und Toleranzwerten.

![VIF Plot](assets/vif_plot.png)



---

## 📈 Modellbewertung

Die Modelle wurden bewertet mit:

- Genauigkeit
- Sensitivität
- Spezifität
- Cohen-Kappa-Score
- ROC-Kurve
- Konfusionsmatrix

---

##  Vergleich der ROC-Kurven

Vergleich der Modellleistung mit ROC-AUC.

![ROC Curve](assets/roc_curve.png)

---

##  Konfusionsmatrix

### Random Forest

![RF Confusion Matrix](assets/confusion_matrix_rf.png)

### AdaBoost

![AdaBoost Confusion Matrix](assets/confusion_matrix_adb.png)

### XGBoost

![XGBoost Confusion Matrix](assets/confusion_matrix_xgb.png)

---

##  Wichtigkeit der Merkmale

Merkmalswichtigkeit aus dem Random-Forest-Modell.

![Feature Importance](assets/feature_importance.png)

---

##  Gespeicherte Modelle

Die trainierten Modelle sind gespeichert in:

```text
model_pkl/
```

Gespeicherte Dateien:

```text
RandomForest_model.pkl
AdaBoost_model.pkl
XGBoost_model.pkl
```

---

##  Projekt lokal ausführen

Repository klonen:

```bash
git clone <repo-url>
cd ML_Flood_Prediction
```

Abhängigkeiten installieren:

```bash
pip install -r requirements.txt
```

Notebook-Skripte ausführen.

---

##  Verwandtes Projekt

Webanwendung für Deployment:
[ML Flood Prediction Website](https://github.com/ololades/ML_Flood_Prediction_Website)

---
