# Projecte de Machine Learning: Kaggle Playground Series S4E8 - Mushroom Classification

Aquest projecte utilitza el dataset del concurs [Playground Series S4E8](https://www.kaggle.com/competitions/playground-series-s4e8/submissions) organitzat per Kaggle. La competició implica desenvolupar models de Machine Learning per a la classificació binària utilitzant un dataset proporcionat per Kaggle.

## ✨ Descripció del projecte

El projecte explora i optimitza dos dels models més potents en Machine Learning: **CatBoost** i **XGBoost**. Es fan servir diferents tècniques d'optimització i ajust de paràmetres per aconseguir el millor rendiment possible en la competició, juntament amb un preprocessament de les dades abastant el tractament de outliers, valors "null", codificació tant de característiques categòriques com ordinals i el target, eliminació de columnes no rellevant a partir de la correlació amb la variable objectiu i la normalització del dataset.

---

## 📝 Contingut del projecte

Conté els notebooks i un arxiu amb les direccions tant a la base de dades com la pàgina de kaggle d'on s'ha obtingut.

---

## ⚙️ Models utilitzats

1. **XGBoost**:
   - Model basat en gradient boosting.
   - Utilitzat amb ajustos d'hiperparàmetres com `n_estimators`, `max_depth` i `learning_rate`.

2. **CatBoost**:
   - Model basat en gradient boosting amb suport natiu per a variables categòriques.
   - Implementat amb paràmetres ajustables com `iterations`, `depth`, i `bagging_temperature`.

---

## 📂 Requeriments

Aquest projecte utilitza **Python** i diverses biblioteques. Assegura't de tenir-les instal·lades:

```bash
pip install catboost xgboost pandas numpy scikit-learn matplotlib