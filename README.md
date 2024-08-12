# Biometric-Authentication-Using-Facial-Recognition
## Project Summary
This project showcases the implementation of a face recognition system based on the Eigenface approach. Face recognition is a crucial technology with applications in various domains such as image and film processing, human-computer interaction, criminal identification, and biometric authentication. The Eigenface method is a well-known technique that simplifies and accelerates face recognition, especially in constrained environments.

The core idea behind the Eigenface approach is to decompose face images into a set of characteristic features, called 'eigenfaces,' which represent the principal components of the training set of face images. These eigenfaces capture the variations among different faces and allow for efficient face recognition by projecting new face images into a reduced subspace called 'face space.' The system then classifies the face by comparing its position in this space with known faces.

## Table of Contents
1. [Motivation](#motivation)
2. [Project Details](#project-details)
   - [Technologies Used](#technologies-used)
   - [Behaviour Algorithms](#behaviour-algorithms)
3. [Limitations](#limitations)
4. [Future Scope](#future-scope)
5. [Conclusion](#conclusion)

## Motivation
With the growing reliance on digital authentication and the increasing need for secure and user-friendly identification methods, biometric authentication has become essential. Traditional methods like passwords and access cards have significant drawbacks, such as being vulnerable to theft, duplication, and security breaches. In contrast, biometric systems offer a more reliable solution by utilizing unique human traits that are difficult to replicate.The face is one of the most acceptable objects for biometrics study and it has also been
the most common method of recognition that human use in their visual interactions. The problem with authentication systems based on fingerprint, voice, iris and the most recent
gene structure (DNA fingerprint) has been the problem of data acquisition. The method of acquiring face images is non-intrusive and thus face can be used as a biometric trait for
covert (where user is unaware that he is being subjected) system.

This project aims to implement a face recognition model that can accurately identify individuals under various conditions, including frontal views, angled views, and scaled images. The Eigenface approach provides a robust framework for developing such a model, making it an excellent choice for applications requiring secure and efficient face recognition. This repository serves as a demonstration of the Eigenface technique and its potential for real-time biometric authentication systems.

## Project Detail
The system is built with a modular architecture, consisting of preprocessing, feature extraction, and matching modules. Each module plays a crucial role in ensuring high accuracy and reliability.

### Architecture and Components
- **Preprocessing Module**
**Noise Removal:** Removes distortions from input images caused by various factors, such as atmospheric conditions or imaging equipment.<br />
**Image Conversion:** Converts JPEG images to a monochromatic format, where each pixel is represented by a single bit (black or white), to simplify further processing.<br />
**Edge Detection:** Uses edge detection algorithms to outline the boundaries of the face, creating a binary matrix that highlights face contours for feature extraction.

- **Feature Extraction Module**
**Dimensional Measurements:** Measures the face's length and width at various points, providing critical data for distinguishing between individuals.<br />
**Perimeter Calculation:** Computes the face's perimeter to enhance recognition accuracy by adding more detailed information to the feature set.
  
- **Matching Module**
**Feature Comparison:** Compares the features extracted from a new image with those stored in the database to determine similarity.<br />
**Threshold-Based Authentication:** Uses a predefined threshold to decide whether the match score indicates successful authentication or rejection.
  
## Features
**Advanced Face Recognition:** Utilizes sophisticated algorithms to accurately authenticate users based on unique facial features.<br />
**Modular Design:** Composed of three distinct modules (Preprocessing, Feature Extraction, and Matching), allowing for clear separation of tasks and ease of integration.<br />
**Noise Reduction:** Incorporates noise removal techniques to enhance the quality of input images, ensuring more reliable feature extraction.<br />
**Binary Image Processing:** Transforms images into a binary format for efficient processing and feature extraction.<br />
**Edge Detection:** Employs edge detection to focus on the facial boundaries, which helps in extracting meaningful features.<br />
**Dimensional and Perimeter Features:** Extracts essential facial dimensions and perimeter to build a comprehensive feature profile of the face.<br />
**Dynamic Thresholding:** Allows for the adjustment of authentication thresholds based on empirical data to optimize system performance.<br />
**Euclidean Distance Metrics:** Uses Euclidean distance to measure feature similarity, facilitating precise face matching and classification.<br />
**Adaptability and Update Capability:** Supports the addition of new face images and recalculation of eigenfaces to keep the system current and accurate.<br />
**User-Friendly Results:** Provides clear pass/fail results based on match scores, making it straightforward for users to understand authentication outcomes.

## Mathematical Foundations
**Principal Component Analysis (PCA):** Utilizes PCA to reduce dimensionality and compute eigenfaces, which represent the key facial features.<br />
**Distance Metrics:** Measures the Euclidean distance between feature vectors to evaluate and match facial features effectively.

