# **Pneumonia Detection Using Convolutional Neural Network (CNN)**

---

## **Problem Statement**

Pneumonia is a serious respiratory disease that affects the lungs and can be life-threatening if not diagnosed at an early stage. Traditional diagnosis through chest X-ray analysis requires expert radiologists and can be time-consuming. There is a need for an automated system that can assist in detecting pneumonia accurately using medical imaging.

---

## **Objective**

The main objective of this project is to develop a deep learning–based image classification model that can automatically identify whether a chest X-ray image belongs to a **normal patient** or a **patient affected by pneumonia**. The system aims to improve diagnostic efficiency and reduce manual effort.

---

## **Dataset Description**

The dataset consists of chest X-ray images categorized into two classes:

* **NORMAL** – X-ray images of healthy lungs
* **PNEUMONIA** – X-ray images showing pneumonia infection

The dataset is organized into three folders:

* Training set
* Validation set
* Test set

Each folder contains subfolders for the two classes. All images are in JPEG format and are resized during preprocessing for model compatibility.

---

## **Methodology / Approach**

1. **Data Loading**
   Chest X-ray images are loaded from directory structures using image data generators.

2. **Preprocessing**

   * Image rescaling for normalization
   * Resizing images to a fixed dimension
   * Conversion into batches for efficient training

3. **Model Architecture**

   * Convolutional Neural Network (CNN) with multiple convolution layers
   * Max pooling layers to reduce spatial dimensions
   * Fully connected (dense) layers for classification
   * Regularization and early stopping to prevent overfitting

4. **Model Training**

   * Binary cross-entropy loss function
   * Adam optimizer
   * Training monitored using validation loss

5. **Evaluation**

   * Model accuracy and loss visualization
   * Performance evaluation on test data
   * Classification report generation

6. **Prediction & Visualization**

   * Predicting class labels for test images
   * Displaying predicted vs actual labels on sample X-ray images

---

## **Tools & Technologies Used**

* **Python 3**
* **TensorFlow / Keras**
* **NumPy**
* **Matplotlib**
* **PIL (Python Imaging Library)**
* **Scikit-learn**
* **Google Colab / Jupyter Notebook**

---

## **Steps to Run the Project**

1. Clone the repository:

   ```bash
   git clone <repository-link>
   ```

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Ensure the dataset folder follows this structure:

   ```
   chest_xray/
   ├── train/
   ├── val/
   └── test/
   ```

4. Run all notebook cells sequentially.

5. The model will train automatically and display performance metrics and predictions.

6. The trained model will be saved locally as:

   ```
   pneumonia_detection.h5
   ```

---

## **Results / Output**

* The CNN model successfully classifies chest X-ray images into **Normal** and **Pneumonia** categories.
* Training and validation accuracy improve steadily across epochs.
* Performance metrics such as accuracy, loss, F1-score, and classification report are generated.
* Sample test images are displayed with predicted and actual labels.
* The trained model is saved for future inference or deployment.
