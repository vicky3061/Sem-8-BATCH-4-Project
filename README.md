# Cleanse AI: Automated Data Preprocessing Tool

Cleanse AI is a Python-based data preprocessing pipeline that automates and standardizes the preparation of raw datasets for machine learning applications. The system intelligently detects and handles missing values, outliers, inconsistent formats, and categorical encoding, while performing feature scaling, selection, and basic text cleaning. With built-in visual analytics, Cleanse AI improves data quality, boosts model performance, and reduces manual preprocessing efforts.

## 🔧 Features

- Automatic handling of missing values using mean, median, or KNN imputation  
- Detection and removal of outliers using Z-Score or Isolation Forest  
- Label and one-hot encoding for categorical variables  
- Min-Max normalization and Standard scaling for numerical features  
- Basic NLP preprocessing: tokenization, stopword removal, and lowercasing  
- Feature selection using statistical tests (Chi-square, ANOVA)  
- Interactive visualizations for data distribution, correlations, and outlier detection  
- Modular and reusable pipeline structure for different datasets  
- CLI support for batch processing of CSV files  
- Optional voice-guided feedback (experimental)

## 🛠 Technologies Used

- Python 3.8+  
- Pandas, NumPy – for data manipulation  
- Scikit-learn – for preprocessing, imputation, and feature selection  
- Matplotlib, Seaborn – for data visualization  
- NLTK / SpaCy – for basic NLP operations  
- Pyttsx3 / SpeechRecognition – for voice interaction (optional)  

## 📁 Project Structure

```
cleanse_ai/
│
├── main.py                    # Entry point for the pipeline
├── modules/
│   ├── missing_value_handler.py
│   ├── outlier_detector.py
│   ├── categorical_encoder.py
│   ├── scaler.py
│   ├── feature_selector.py
│   └── visualizer.py
├── examples/
│   └── sample_dataset.csv
├── utils/
│   └── data_loader.py
├── README.md
└── requirements.txt
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/cleanse-ai.git
cd cleanse-ai
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Preprocessing Pipeline

```bash
python main.py --input examples/sample_dataset.csv --output output/cleaned_data.csv
```

## ⚙️ Configuration Options

| Argument        | Description                              |
|----------------|------------------------------------------|
| `--input`       | Path to the input CSV file               |
| `--output`      | Output path for cleaned dataset          |
| `--voice`       | Enable voice feedback (default: False)   |

## 🧪 Sample Use Case

Cleanse AI was tested on multiple academic and real-world datasets including student performance data, retail transaction logs, and healthcare records. In all cases, the tool successfully improved model accuracy by reducing noise and ensuring consistent input formats.

## 🤖 Future Enhancements

- Integration with cloud storage (e.g., AWS S3, Google Drive)  
- Support for time-series preprocessing  
- AutoML recommendations for preprocessing strategies  
- GUI-based desktop version

## 📜 License

This project is licensed under the MIT License.

## 🙌 Acknowledgments

Thanks to the academic team at [Your Institution] and the contributors from the iZEN Training Academy for support during project development.
