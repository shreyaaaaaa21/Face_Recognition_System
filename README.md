<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
      

  <h1>Facial Recognition Project</h1>
    <p>This project implements a facial recognition system using the <strong>Local Binary Pattern Histogram (LBPH)</strong> algorithm. The system detects faces, processes images, and predicts labels based on training data.</p>

  <h2>Features</h2>
    <ul>
        <li>Face detection using OpenCV's Haar Cascade Classifier.</li>
        <li>Facial recognition using the LBPH algorithm.</li>
        <li>Training and testing images are processed in grayscale for better performance.</li>
        <li>Real-time prediction of the subject's name based on input images.</li>
        <li>Displays the confidence score for each prediction.</li>
        <li>Handles unknown labels gracefully with fallback to "Unknown" label.</li>
    </ul>

  <h2>Algorithm Used: Local Binary Pattern Histogram (LBPH)</h2>
    <p>The LBPH algorithm is a simple yet efficient method for facial recognition. It works by analyzing the pixel intensity patterns in small neighborhoods around each pixel, converting these into a histogram, and then matching the histograms between the test and training images.</p>

  <h2>Steps Involved in the Project</h2>
    <ol>
        <li><strong>Data Preparation:</strong> Faces are detected and extracted from training images using the Haar Cascade Classifier, converted into grayscale, and then stored with corresponding labels.</li>
        <li><strong>Training:</strong> The extracted faces are used to train the LBPH recognizer. Labels are mapped to the names of the subjects.</li>
        <li><strong>Prediction:</strong> Test images are processed to predict the subject's identity. If the model fails to recognize a face, it labels it as "Unknown".</li>
        <li><strong>Result Visualization:</strong> The predicted labels and confidence scores are drawn on the test images.</li>
    </ol>

  <h2>How to Run</h2>
    <pre>
    1. Prepare the training data folder, each containing labeled images of different subjects.
    2. Modify the paths in the script to point to your data folders.
    3. Upload the training images folder to the specified location in Google Colab.
    4. Train the LBPH recognizer using the prepared dataset.
    5. Use the trained model to predict on test images.
    6. View predictions using `cv2_imshow` (for Colab).
    </pre>

  <h2>Technologies and Libraries</h2>
    <ul>
        <li><strong>Python:</strong> The programming language used for the project.</li>
        <li><strong>OpenCV:</strong> For face detection, image processing, and visualization.</li>
        <li><strong>LBPH Recognizer:</strong> The algorithm used for facial recognition.</li>
        <li><strong>Google Colab:</strong> For training and testing the model.</li>
    </ul>

</body>
</html>
