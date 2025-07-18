Brain Tumor Detection and Classification Application 🧠💻
Overview 🌟
This MATLAB application provides a user-friendly graphical user interface (GUI) for automated brain tumor detection and classification from medical imaging data 📸. It supports the full pipeline of image processing, including browsing, preprocessing, segmentation, feature extraction, and classification using various machine learning algorithms 🤖. Designed to assist researchers and medical professionals, this tool simplifies brain tumor analysis with an intuitive interface 😊.
Features ✨

Image Loading 📂: Load medical images (JPG, JPEG, PNG, BMP) or use default datasets for tumor types like Tuberculoma, Granuloma, Astrocitoma, Schwannoma, and Meningioma.
Preprocessing 🛠️: Resize images to 256x256 pixels, convert to grayscale, and enhance quality with intensity adjustments.
Segmentation 🔍: Segment tumor regions using adaptive thresholding and k-means clustering, with visualization of tumor boundaries and metrics like volume, width, height, and depth 📏.
Feature Extraction 📊: Compute image features such as Contrast, Entropy, Mean, Variance, and RMS for classification.
Classification 🧠: Use algorithms like Quadratic SVM, Boosted Tree, Cubic SVM, Linear SVM, Random Forest, and KNN, with performance metrics (Accuracy, Precision, Recall, F1-Score, Specificity, Sensitivity) displayed 📈.
Algorithm Comparison ⚖️: Visualize algorithm performance with a bar graph for easy comparison.
Result Analysis 🔬: Identify tumor types based on folder names and display their distribution.
Clear and Exit Options 🧹: Reset all data or close the application with a single click.

Installation 🛠️

Ensure MATLAB (R2018b or later) is installed on your system 🖥️.
Clone or download this repository to your local machine 📥.
Install the MATLAB Image Processing Toolbox for image handling and feature extraction 📷.
Place your dataset in a Dataset folder with subfolders for each tumor type (e.g., Tuberculoma T2, Granuloma T1C+, etc.) or use the default image paths provided 📂.

Usage 🚀

Open MATLAB and navigate to the directory containing the code.
Run the brainTumorDetectionApp function to launch the GUI 🎉.
Follow these steps in the GUI:
Browse Input Image 📷: Select an image or load default dataset images.
Preprocessing 🖌️: Enhance the selected image for analysis.
Segmentation 🧩: Segment the tumor and view the results.
Feature Extraction 📈: Extract features for classification.
Select Feature 🔍: Confirm feature selection (placeholder for future enhancements).
Classification 🤖: Choose an algorithm and classify the tumor.
Analysis 🔬: Review tumor type distribution across loaded images.
Comparison 📊: Compare algorithm accuracies in a bar graph.
Clear All 🧹: Reset all data and GUI fields.
Exit 🚪: Close the application.



Dataset 📁
The application expects a dataset in a Dataset/test directory with subfolders:

Tuberculoma T2
Granuloma T1C+
Astrocitoma T1C+
Schwannoma T1C+
Meningioma T1C+

Each subfolder should contain images (e.g., image1.jpeg, second1.jpeg, etc.) for the respective tumor type. Default images are loaded if no image is manually selected 📸.
Requirements ⚙️

MATLAB R2018b or later
MATLAB Image Processing Toolbox
A dataset of brain tumor images organized as described above 📂

Notes 📝

Classification metrics (Accuracy, Precision, Recall, F1-Score, Specificity, Sensitivity) are simulated with random values for demonstration purposes 🎲. Replace with trained models for real-world use.
Tumor depth is simplified to 10 units for volume calculations 📏. Adjust for 3D imaging data as needed.
Error handling ensures proper workflow (e.g., selecting an image before preprocessing) 🚨.

Future Improvements 🔮

Integrate trained machine learning models for accurate classification 🤖.
Support 3D medical imaging formats (e.g., DICOM) for precise tumor analysis 🧠.
Enhance feature selection with advanced algorithms or user-defined options ⚙️.
Add export functionality for results and segmented images 📤.
Optimize for large datasets and real-time processing ⏩.

License 📜
This project is licensed under the MIT License. See the LICENSE file for details.
Contact 📬
For questions or contributions, open an issue or submit a pull request on the GitHub repository 🙌.
