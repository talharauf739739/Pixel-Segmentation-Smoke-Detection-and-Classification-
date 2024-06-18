# Pixel-Segmentation-Smoke-Detection-and-Classification-
In this project, I developed a comprehensive system for detecting and classifying smoke intensity in 
images using advanced machine learning techniques. The dataset, sourced from the Kaggle platform, 
consisted of smoke-containing images which were annotated using the Roboflow platform, following the 
YOLO V8 annotation format. The preprocessing phase involved detecting and drawing bounding boxes 
around smoke regions using the YOLO V8 model, followed by applying various augmentation techniques 
such as flipping, rotation, translation, and blurring to enhance the dataset. Regions of interest (ROIs) 
were then extracted from the augmented images, retaining only those that accurately detected specific 
annotated areas. For classification, the system labeled the images as either "High Smoke" or "Low 
Smoke" based on the pixel intensity within the bounding boxes, using a function that calculated the 
average intensity. A Convolutional Neural Network (CNN) was employed for the binary classification 
task, with the dataset split into 80% for training and 20% for testing. The model was trained with specific 
parameters, and ensemble learning was implemented by training three separate CNN models to 
improve robustness. The ensemble model achieved an impressive accuracy score of 0.99 after 20 
epochs. Cross-validation and entropy loss tests were conducted, resulting in a mean cross-validated 
accuracy of 0.9890 and a mean entropy loss of 0.0406. This rigorous approach ensured the development 
of a highly accurate and reliable model, suitable for practical applications such as environmental 
monitoring and fire detection
