# **MEDICO - Medical Image Analysis**


## Summary of the project
1. Developed a classification model using convolutional neural network to classify the medical images according to image type (MRI, X-ray, CT scan) and body parts (Brain, Knee, Shoulder)
- Loaded the dataset using the python library "argparse"
- pre-processed the images by resizing the input images to 32X32 and then scaling the data points from [0, 255] (the minimum and maximum RGB values of the image) to the range [0, 1]
- Instantiated the Convolutional Neural Network to train the image classifier
- The calculated accuracy on testing data : 95%

2. Perform text recognition on medical images using OpenCV’s EAST deep learning model for text detection and tesseract
- Used OpenCV’s EAST text detector to detect the presence of text in an image which helped us to locate the bounding box (x, y)-coordinates of text ROIs.
- extracted each of these ROIs and then passed them into Tesseract v4’s LSTM deep learning text recognition algorithm to gain actual OCR(Optical Character Recognition) results

3. Implemented an ER model and created database consisting of 15 tables on MySQL workbench and linked it with machine learning models using MySQL connector
