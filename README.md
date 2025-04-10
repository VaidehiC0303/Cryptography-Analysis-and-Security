## 🔐 Cryptanalysis , Weakness Detection & Recommendation model

This project focuses on analyzing cipher text and detecting weaknesses in encryption schemes using machine learning techniques. It involves extracting statistical features from cipher data and training classifiers to predict the type of cipher or identify vulnerabilities.

---

### 📁 Dataset

The dataset used is a CSV file: `updated_large_meaningful_cipher_dataset.csv`.  
It contains ciphered texts along with associated keys and labels describing the type of encryption used.

---

### 📊 Feature Engineering

The notebook extracts several key features from the cipher data:

- **Key Entropy & Cipher Entropy**: Measures randomness using Shannon entropy.
- **Key Length & Cipher Length**: Captures the size of the encryption components.
- **Key to Cipher Ratio**: Ratio of key length to cipher length.
- **Entropy Ratio**: Ratio of key entropy to cipher entropy.

These features are designed to capture statistical patterns useful for classification.

---

### 🧠 Machine Learning Models

Several classifiers are trained and evaluated to classify or assess cipher weaknesses:

- `RandomForestClassifier`
- `XGBClassifier` (XGBoost)
- `LGBMClassifier` (LightGBM)
- `VotingClassifier` (Ensemble of the above models)

Models are evaluated using:
- Accuracy
- Classification report (Precision, Recall, F1-score)

---

### 🧪 Usage

To run the notebook:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/cryptanalysis-weakness-detection.git
   cd cryptanalysis-weakness-detection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   Open `crypt_analysis&weakness detection.ipynb` in Jupyter Notebook or VSCode and run all cells.

---

### 📦 Dependencies

- pandas
- numpy
- scikit-learn
- xgboost
- lightgbm
- scipy


