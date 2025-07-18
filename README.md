Brain Tumor Detection and Classification Application

Overview

This MATLAB application provides a graphical user interface (GUI) for automated brain tumor detection and classification from medical imaging data. It supports the entire pipeline of image processing, including browsing and loading images, preprocessing, segmentation, feature extraction, and classification using various machine learning algorithms. The application is designed to assist researchers and medical professionals in analyzing brain tumor images efficiently.

Features





Image Loading: Supports browsing and loading medical images in formats such as JPG, JPEG, PNG, and BMP. Default datasets for various tumor types (Tuberculoma, Granuloma, Astrocitoma, Schwannoma, Meningioma) are included.



Preprocessing: Resizes images to 256x256 pixels and converts them to grayscale for consistency. Applies intensity adjustment to enhance image quality.



Segmentation: Uses adaptive thresholding and k-means clustering to segment potential tumor regions. Displays segmented tumor boundaries and calculates metrics like volume, width, height, and depth.



Feature Extraction: Computes image features such as Contrast, Entropy, Mean, Variance, and RMS (Root Mean Square) for use in classification.



Classification: Supports multiple machine learning algorithms, including Quadratic SVM, Boosted Tree, Cubic SVM, Linear SVM, Random Forest, and KNN. Displays performance metrics such as Accuracy, Precision, Recall, F1-Score, Specificity, and Sensitivity.



Algorithm Comparison: Visualizes the performance of different classification algorithms in a bar graph for comparative analysis.



Result Analysis: Identifies tumor types based on folder names and provides a distribution of tumor types across loaded images.



Clear and Exit Options: Allows resetting all data and closing the application.

Installation





Ensure MATLAB (version R2018b or later) is installed on your system.



Clone or download the repository to your local machine.



Ensure the MATLAB Image Processing Toolbox is installed for image handling and feature extraction functions.



Place the dataset in a folder named Dataset with subfolders for each tumor type (e.g., Tuberculoma T2, Granuloma T1C+, etc.), or use the provided default image paths.

Usage





Open MATLAB and navigate to the directory containing the application code.



Run the brainTumorDetectionApp function to launch the GUI.



Follow these steps in the GUI:





Browse Input Image: Select an image or use default images from the dataset.



Preprocessing: Preprocess the selected image to enhance quality.



Segmentation: Segment the tumor region and view the results.



Feature Extraction: Extract image features for classification.



Select Feature: Confirm feature selection (placeholder for future feature selection logic).



Classification: Choose a machine learning algorithm and classify the tumor.



Analysis: Analyze tumor types across loaded images.



Comparison: Compare the accuracy of different algorithms after classification.



Clear All: Reset all data and GUI fields.



Exit: Close the application.

Dataset

The application expects a dataset organized in a Dataset/test directory with subfolders for each tumor type:





Tuberculoma T2



Granuloma T1C+



Astrocitoma T1C+



Schwannoma T1C+



Meningioma T1C+

Each subfolder should contain images (e.g., image1.jpeg, second1.jpeg, etc.) for the respective tumor type. The application automatically loads default images if no image is manually selected.

Requirements





MATLAB R2018b or later



MATLAB Image Processing Toolbox



A dataset of brain tumor images organized as described above

Notes





The classification metrics (Accuracy, Precision, Recall, F1-Score, Specificity, Sensitivity) are simulated using random values within reasonable ranges for demonstration purposes. In a production environment, these should be replaced with actual trained machine learning models.



The application assumes a simplified tumor depth of 10 units for volume calculations. This can be adjusted based on actual 3D imaging data.



Error handling is implemented to ensure the user selects an image, preprocesses it, and extracts features before classification.

Future Improvements





Integrate trained machine learning models for accurate classification.



Support 3D medical imaging formats (e.g., DICOM) for more precise tumor analysis.



Enhance feature selection with advanced algorithms or user-defined options.



Add export functionality for results and segmented images.



Optimize performance for large datasets and real-time processing.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Contact

For questions or contributions, please open an issue or submit a pull request on the GitHub repository.
