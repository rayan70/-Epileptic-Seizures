

## 🧠 EEG-Based Epileptic Seizure Prediction

This project aims to predict epileptic seizures and detect brain anomalies (like tumors) using EEG signal analysis and machine learning techniques.

### 📌 Objective

* Predict epileptic seizures from EEG time-series data.
* Distinguish between brain states (healthy, tumor-affected, epileptic activity).
* Support early diagnosis and improve patient treatment strategies.

### 🧪 Dataset

* EEG recordings from 500 subjects, each with 4097 data points over 23.6 seconds.
* Data segmented into 11,500 samples of 178 features (1 second each).
* Labels (1–5) represent different brain states:

  * `1`: Epileptic seizure
  * `2`: Tumor area
  * `3`: Healthy brain near tumor
  * `4`: Eyes closed
  * `5`: Eyes open
  * https://www.kaggle.com/datasets/harunshimanto/epileptic-seizure-recognition

### 🔍 Methodology

* **CRISP-DM** process for structured data science workflow.
* Feature extraction using:

  * **Discrete Wavelet Transform (DWT)**
  * **Autoregressive (AR) models**
* Models trained and compared:

  * `Decision Tree`
  * `k-Nearest Neighbors (k-NN)`
  * `Support Vector Machines (SVM)`
  * `Logistic Regression`
  * `Artificial Neural Networks (ANN)`
  * `Recurrent Neural Networks (RNN)`
  * `XGBoost`

### 🏆 Results

* Best performance achieved by: `k-NN`, `ANN`, and `SVM`.
* RNNs provided promising results for sequential pattern learning.
* Evaluation used confusion matrices and accuracy metrics.
* UMAP and KMeans used for visualization and clustering.

### 🛠 Tools & Libraries

* `Python`, `Pandas`, `NumPy`, `Scikit-learn`, `TensorFlow`, `Keras`, `Matplotlib`, `Seaborn`, `XGBoost`, `Pyngrok`, `Flask`

### 🚀 Deployment

* API created with **Flask**.
* Local and remote testing enabled via **Pyngrok**.

