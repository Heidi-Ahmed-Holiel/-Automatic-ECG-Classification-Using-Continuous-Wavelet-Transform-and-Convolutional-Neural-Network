# -Automatic-ECG-Classification-Using-Continuous-Wavelet-Transform-and-Convolutional-Neural-Network

We've developed a system that employs CWT for feature extraction from ECG signals and CNNs for classification. The system is trained and tested on ECG data to accurately classify it into Arrhythmia (ARR), Congestive Heart Failure (CHF), and Normal Sinus Rhythm (NSR).

The dataset repo link: https://github.com/mathworks/physionet_ECG_data/

## Technical Details

- **Continuous Wavelet Transform (CWT)**: We use CWT for efficient feature extraction from ECG signals, facilitating a better representation in both time and frequency domains.
- **Scalogram Generation**: Scalograms are generated as a visual representation of CWT coefficients. This is particularly useful for handling noisy ECG signals.
- **Convolutional Neural Networks (CNN)**: CNNs are employed for their efficacy in image classification, here used to classify the scalogram images into different heart disease categories.

## Data Preprocessing and Analysis

- ECG data is read and preprocessed, including segmenting signals into training and validation data.
- Scalogram images are generated from the ECG signals.

## Pretrained Models and Customization

- **AlexNet**: Used for initial trials with customizations to suit ECG signal data.
- **VGG-16**: Employed for its deep architecture, providing enhanced feature recognition.
- **Inception-V3**: Utilized for its efficiency in handling larger image sizes.
- **SqueezeNet**: Tested for its compact architecture and speed.

## Results

- The performance of each model is evaluated based on accuracy and computational efficiency.
- VGG-16 emerged as the most accurate model with accuracy 88%, albeit with higher computational demands.

## Conclusion

This project demonstrates the potential of using CWT and CNNs for effective ECG signal classification. VGG-16, despite its computational intensity, provides the highest accuracy, showcasing the trade-off between computational demand and classification performance.
