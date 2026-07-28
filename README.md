# ml-products_analysis
Created Machine Learning model deigned to automatically classify products into their respective categories using product titles and advanced text-based engineered features.
This project follows strict industry data team standards, ensuring reproducibility, clear versioning, and seamless collaborative handovers.
## Data Pipeline & Feature Engineering
The system doesn't rely solely on raw text frequencies. To maximize precision, the data pipeline extracts structural signals from the product titles:
- Text Standardization: Lowercasing, noise reduction, and handling missing/empty title entries safely.
- Text Vectorization: TF-IDF representation capturing critical unigrams and bigrams.
- Engineered Structural Features:
  -  Word & Character Counts: Measuring the length and verbosity of the titles.
  - Numeric & Special Character Density: Flagging technical dimensions or specifications (e.g., "12V", "3.5mm").
  - Capitalization Patterns: Identifying potential brand names or technical acronyms written in uppercase (e.g., USB, LED, HD).
  - Maximum Word Length: Spotting long descriptive compounds or serial strings.
## Model Development & Evaluation
During exploration, multiple machine learning architectures were benchmarked to find the optimal trade-off between speed, interpretability, and predictive performance (e.g., Logistic Regression, Linear Support Vector Classification, and Random Forest Ensembles).
Models are strictly evaluated using:
  - Overall Accuracy
  - Classification Report (Precision, Recall, and F1-Score calculated per product category)
  - Confusion Matrix Visualization to pinpoint exactly where the model struggles or misclassifies items
# Usage Instructions
## Training the Model
- Model training is performed on the provided dataset and the mist successful model is further used for testing.
## Testing the Model
- Selected model is used for testing on different products form dataset and from user input
- Model's success has been discussed based on the achieved results
