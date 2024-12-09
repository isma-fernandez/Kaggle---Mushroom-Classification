# Projecte de Machine Learning: Kaggle Playground Series S4E8 - Mushroom Classification

Aquest projecte utilitza el dataset del concurs [Playground Series S4E8](https://www.kaggle.com/competitions/playground-series-s4e8/submissions) organitzat per Kaggle. La competició implica desenvolupar models de Machine Learning per a la classificació binària utilitzant un dataset proporcionat per Kaggle.

## ✨ Descripció del projecte

El projecte explora i optimitza tres dels models més potents en Machine Learning: **CatBoost**, **XGBoost** i **LightGBM**. També es desenvolupen experiments amb altres algoritmes per contrastar el rendiment i trobar una combinació òptima. Es fan servir diferents tècniques d'optimització i ajust de paràmetres per aconseguir el millor rendiment possible en la competició, juntament amb un preprocessament de les dades abastant el tractament de outliers, valors "null", codificació tant de característiques categòriques com ordinals i el target, eliminació de columnes no rellevant a partir de la correlació amb la variable objectiu i la normalització del dataset.

---

## 📝 Contingut del projecte

Conté els notebooks amb experiments detallats que implementen:
- Divisió de dades amb `train_test_split` i estratègies avançades com `StratifiedKFold`.
- Codificació utilitzant eines com `LabelEncoder`, `OrdinalEncoder` i `OneHotEncoder`.
- Normalització i escalat amb `StandardScaler`.
- Selecció i transformació de característiques amb tècniques com PCA (Anàlisi de Components Principals).

---

## ⚙️ Models utilitzats

1. **XGBoost**:
   - Model basat en gradient boosting.
   - Utilitzat amb ajustos d'hiperparàmetres com `n_estimators`, `max_depth` i `learning_rate`.

2. **CatBoost**:
   - Model basat en gradient boosting amb suport natiu per a variables categòriques.
   - Implementat amb paràmetres ajustables com `iterations`, `depth`, i `bagging_temperature`.

3. **LightGBM (LGBM)**:
   - Model optimitzat per a grans datasets i alta velocitat d'entrenament.
   - Ajustos d'hiperparàmetres com `num_leaves`, `max_depth`, i `learning_rate`.
   - Implementació nativa de Gradient Boosting Decision Tree (GBDT).

4. **Altres models explorats**:
   - **Logistic Regression**: Base lineal.
   - **Random Forest**: Model d'ensemble basat en arbres de decisió.
   - **Support Vector Machines (SVM)**: Algoritme lineal i no lineal.
   - **Decision Trees**: Model explicatiu per característiques simples.

---

## ⚙️ Metodologies d'Avaluació

- Mètriques:
  - `accuracy_score`, `f1_score`, i `matthews_corrcoef` per analitzar el rendiment.
- Cross-validation:
  - Implementada amb `cross_val_score` i CV específic per XGBoost (`xgb_cv`), CatBoost (`catboost_cv`) i LightGBM (`lgb.cv`).

---

## 📂 Requeriments

Aquest projecte utilitza **Python** i diverses biblioteques. Assegura't de tenir-les instal·lades:

```bash
pip install catboost xgboost lightgbm pandas numpy scikit-learn matplotlib