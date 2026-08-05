# 🌭 Hot Dog or Not Hot Dog? (CNN Image Classification)

This project is an **Image Classification** model inspired by the iconic app from the TV show *Silicon Valley*. The goal of this project is to use artificial intelligence to detect whether a given food photo is a "Hot Dog" or "Not Hot Dog".

The model was built and trained from scratch using a **Convolutional Neural Network (CNN)** architecture.

## 🚀 Project Overview & Features

*   **Dataset:** The massive [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) dataset was used, but it was filtered and converted into a binary classification problem by separating hot dogs from the rest of the food categories.
*   **Data Augmentation:** To prevent the model from memorizing the training images (overfitting), random transformations such as rotation, flipping, and scaling were applied to the images during the training phase.
*   **Performance Optimization:** The model was trained on Google Colab using a **T4 GPU**. TensorFlow's `.cache()` and memory management features were utilized to reduce data loading times to mere seconds.
*   **Visualization:** The training process (Accuracy and Loss metrics) and prediction results were visualized using **Matplotlib**.

## 🛠️ Technologies Used

*   **Programming Language:** Python
*   **Deep Learning Libraries:** TensorFlow & Keras
*   **Data Visualization:** Matplotlib
*   **Environment:** Google Colab (Jupyter Notebook)

## 📊 Training Process

*   Before being fed into the model, the images were resized to `128x128` pixels, and their pixel values were normalized to a range between `0.0` and `1.0`.
*   The model was trained for **50 Epochs**.
*   To prevent training interruptions at the end of the dataset batches, a continuous training loop was established using the `.repeat()` and `steps_per_epoch` methods.

## 💻 How to Run

To test this project in your browser without needing to install anything locally:

1. Open the `HotDogvsNotHotDog_ConvolutionalNeuralNet...ipynb` file in this repository.
2. Click the **"Open in Colab"** button at the top of the file.
3. Once Google Colab opens, navigate to the top menu and select **Runtime > Change runtime type**, then set the Hardware accelerator to **T4 GPU**.
4. Run all the cells sequentially (Shift + Enter) to train the model from scratch or inspect the results.

---
*This project was developed as a first step into the world of Deep Learning and CNNs.*
