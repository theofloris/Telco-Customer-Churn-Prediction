# 📊 Telco Customer Churn Prediction: Analisi e Modellazione

## 📝 Descrizione del Progetto
Il **Churn Rate** (tasso di abbandono) è una delle metriche più critiche per le aziende di telecomunicazioni. Acquisire un nuovo cliente costa molto di più che mantenerne uno esistente.
Questo progetto analizza il dataset "Telco Customer Churn" per identificare i comportamenti dei clienti che indicano una propensione all'abbandono. L'obiettivo finale è costruire un modello di Machine Learning capace di prevedere quali utenti sono a rischio, permettendo all'azienda di intervenire con strategie di retention mirate.

## 🚀 Pipeline del Progetto
Il notebook segue un flusso di lavoro end-to-end:

**Data Analysis e Data Cleaning**: Analisi generale del dataset in oggetto, gestione dei valori mancanti (es. TotalCharges), e correzione dei tipi di dato.

**Exploratory Data Analysis (EDA)**: Visualizzazione delle correlazioni tra variabili demografiche, servizi sottoscritti, e tipo di contratto rispetto al Churn.

**Feature Engineering**: Encoding delle variabili categoriche, e scaling dei dati numerici.

**Model Building**: Implementazione dell'algoritmo Random Forest per la predizione 

**Evaluation**: Valutazione basata su metriche di business come Accuracy, Precision, Recall, F1-Score, e AUC.

## 📈 Key Insights (Esempi di Analisi)
Durante l'analisi esplorativa sono emersi alcuni punti chiave:

**Contratti Month-to-month**: I clienti con contratti mensili hanno un tasso di abbandono significativamente più alto.

**Metodo di Pagamento**: Gli utenti che utilizzano il "Electronic check" tendono ad abbandonare più frequentemente.

**Tenure**: I primi 6 mesi sono critici; se un cliente supera il primo anno, la probabilità di churn crolla drasticamente.

## 📊 Risultati del Modello
Il modello finale ha ottenuto le seguenti performance sul test set:
| Metrica | Valore | Note |
| :--- | :--- | :--- |
| **Accuracy** | 0.7957 | Capacità complessiva di indovinare la classe corretta. |
| **Precision** | 0.6625 | Capacità di non classificare come churn chi non lo è. |
| **Recall** | 0.4724 | Capacità di trovare tutti i clienti che abbandoneranno. |
| **F1-Score** | 0.5515 | Media armonica tra Precision e Recall; bilancia il costo dei falsi positivi e dei falsi negativi. |
| **ROC-AUC** | 0.8341 | Capacità del modello di distinguere tra le classi. |

## 🏁 Come Eseguire il Progetto
1. Scarica il dataset [Kaggle: Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data)

2. Clona la repository:
```bash
git clone https://github.com/theofloris/Telco-Customer-Churn-Prediction.git
```

3. Entra nella cartella:
```bash
cd Telco-Customer-Churn-Prediction
```

4. Apri il Notebook, carica il dataset nella stessa cartella (se su IDE). Caricalo nei file (se su Google Colab o Jupyter) Notebook ed esegui la prima cella.
