# 🏆 Sports Celebrity Image Classification

This project builds an image classifier that recognizes five famous sports celebrities using traditional machine learning techniques and image processing. It uses OpenCV for image manipulation, PyWavelets for feature extraction, and Scikit-learn models for classification.

---

## 📌 Objective

To classify images of sports celebrities into one of the following five categories:
- **Lionel Messi**
- **Maria Sharapova**
- **Roger Federer**
- **Serena Williams**
- **Virat Kohli**

---

## 📂 Project Structure

```bash
├── sports_celebrity_classification.ipynb  # Main notebook (modeling & classification)
├── data_cleaning.ipynb                    # Image cleaning and preprocessing
├── class_dictionary.json                  # Mapping of class labels to names
├── requirements.txt                       # Required Python packages
└── README.md                              # Project documentation
⚙️ How It Works
1. Data Collection & Cleaning
Images of each celebrity are collected into separate folders.

Preprocessing includes resizing images to a uniform size (e.g., 32x32), converting to grayscale, and removing corrupted files.

Handled via data_cleaning.ipynb.

2. Feature Extraction
Raw Pixel Features: Flattened grayscale image data.

Wavelet Features: Extracted using PyWavelets to capture frequency and texture information.

Combined to form a comprehensive feature vector for each image.

3. Model Training
Split dataset into training and testing sets.

Trained using Scikit-learn classifiers (e.g., SVM or Random Forest).

Hyperparameter tuning and model selection done manually or via grid search.

4. Evaluation
Evaluated using classification accuracy and confusion matrices.

Results are visualized using Seaborn heatmaps.

🧪 Libraries Used
Install the required libraries using:

bash
Copy
Edit
pip install -r requirements.txt
Requirements:
opencv-python==3.4.3.18

PyWavelets==0.5.2

seaborn==0.8.1

🎯 Class Labels
Class mapping used in this project:

json
Copy
Edit
{
  "lionel_messi": 0,
  "maria_sharapova": 1,
  "roger_federer": 2,
  "serena_williams": 3,
  "virat_kohli": 4
}
📈 Sample Output
Classification accuracy of the model on the test set.

Confusion matrix visualizing model predictions.

Optionally, predictions on new/unseen celebrity images.
