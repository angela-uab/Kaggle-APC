# 🏙️ **Cas Kaggle - Airbnb NYC Open Data**

## **👩‍💻 Autors**
- Àngela Obón Soto (1600359)
- Muniba Liaqat Ali Ali (1635042)

## **📂 Repositori GitHub**
[![GitHub Repo](https://img.shields.io/badge/Repositori-GitHub-blue)](https://github.com/angela-uab/Kaggle-APC.git)

## **📊 Dataset**
[![Dataset Kaggle](https://img.shields.io/badge/Dataset-Kaggle-orange)](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data)

---

## **📖 Descripció del projecte**

Aquest projecte analitza el conjunt de dades d'Airbnb a Nova York per al 2019. L'objectiu és explorar els factors que influeixen en els preus dels llistats (`price`) i en la seva disponibilitat (`availability_365`). Mitjançant l'anàlisi de dades i la construcció de models predictius, es busquen insights rellevants per a amfitrions i usuaris.

### **🎯 Objectius principals**
1. 📌 Analitzar diferències de preus entre barris i tipus d'habitacions.
2. 🔍 Identificar els factors que més influeixen en el preu.
3. 🌐 Explorar patrons de disponibilitat segons àrees geogràfiques.
4. 📈 Estudiar l'activitat dels amfitrions més ocupats.
5. 🤖 Construir models per predir el preu d'un llistat.

---

## **🧹 Exploració i neteja de dades**

### **📌 Variables clau analitzades**
| Variable               | Descripció                                           |
|------------------------|-----------------------------------------------------|
| **`price`**            | Preu per nit (variable objectiu).                   |
| **`room_type`**        | Tipus d'habitació (complet, privat o compartit).    |
| **`neighbourhood_group`** | Zona geogràfica principal (e.g., Manhattan).      |
| **`availability_365`** | Dies disponibles per reservar durant l'any.         |
| **`number_of_reviews`**| Total de ressenyes rebudes pel llistat.             |

### **🔧 Processament**
✅ Eliminació de duplicats.  
✅ Tractament de valors extrems i nuls.  
✅ Codificació de variables categòriques (`room_type`, `neighbourhood_group`).  

---

## **⚙️ Models utilitzats**

| **Model**             | **R² Score** | **MSE (Test)** | **RMSE** | **MAE** | **Temps Entrenament** |
|-----------------------|--------------|----------------|----------|---------|-----------------------|
| Regressió Lineal      | 0.291        | 9568.77        | 97.82    | 57.99   | 0.54s                |
| Random Forest         | 0.377        | 8125.57        | 90.14    | 50.43   | 11.16s               |
| **Gradient Boosting** | **0.393**    | **7917.48**    | **88.98**| **49.82**| 12.73s              |
| Decision Tree         | 0.370        | 8502.85        | 92.21    | 50.69   | 19.99s               |
| KNN                   | 0.408        | 7991.28        | 89.39    | 49.91   | 8.68s                |

**🔑 Model recomanat:**  
🎖️ **Gradient Boosting** ofereix el millor rendiment global.

---

## **📊 Conclusions**

### **📍 Factors clau en el preu**
- **Tipus d'habitació:** Els apartaments complets són significativament més cars que les habitacions privades o compartides.
- **Localització:** Manhattan lidera amb els preus més alts.

### **📍 Patrons de disponibilitat**
- **Queens i Brooklyn** tenen la disponibilitat mitjana més alta (`availability_365`).
- Llistats amb més dies disponibles tendeixen a tenir preus competitius.

### **📍 Insights geoespacials**
- Els barris de **Manhattan** i **Brooklyn** són els més rendibles per als amfitrions.
- La proximitat a zones turístiques té un fort impacte en els preus.

---



  
