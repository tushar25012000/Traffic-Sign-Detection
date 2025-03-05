# Traffic Sign Detection

A Python-based project for detecting and recognizing traffic signs using image processing and machine learning techniques.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

This project aims to detect and classify traffic signs from images, facilitating applications such as driver assistance systems and autonomous vehicles. By leveraging machine learning algorithms, the system identifies various traffic signs to enhance road safety and driving efficiency.

## Features

- Detection of multiple traffic sign types.
- High accuracy in classification.
- Real-time processing capability.

## Dataset

The project utilizes the [LISA Traffic Sign Dataset](https://git-disl.github.io/GTDLBench/datasets/lisa_traffic_sign_dataset/), which includes:

- 47 US sign types.
- 7855 annotations on 6610 frames.
- Sign sizes ranging from 6x6 to 167x168 pixels.
- Images captured from different cameras with varying resolutions.

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/tushar25012000/Traffic-Sign-Detection.git
   cd Traffic-Sign-Detection
   ```

2. **Create a virtual environment (optional but recommended):**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

   Ensure that the following packages are installed:

   - OpenCV
   - NumPy
   - TensorFlow
   - Keras
   - scikit-learn

## Usage

1. **Prepare the dataset:**

   - Download the LISA Traffic Sign Dataset and place it in the `dataset/` directory.
   - Run the preprocessing script to prepare the data for training:

     ```bash
     python preprocess_data.py
     ```

2. **Train the model:**

   ```bash
   python train_model.py
   ```

   This will train the traffic sign detection model using the prepared dataset.

3. **Test the model:**

   ```bash
   python test_model.py
   ```

   Evaluate the model's performance on test data.

4. **Detect traffic signs in new images:**

   ```bash
   python detect_signs.py --image path_to_image.jpg
   ```

   Replace `path_to_image.jpg` with the path to your input image.

## Results

The trained model achieves an accuracy of approximately 95% on the test dataset. Below are some sample detection results:

![Sample Detection 1](images/sample1.jpg)
*Figure 1: Detection of a stop sign.*

![Sample Detection 2](images/sample2.jpg)
*Figure 2: Detection of a pedestrian crossing sign.*

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

Please ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- The [LISA Traffic Sign Dataset](https://git-disl.github.io/GTDLBench/datasets/lisa_traffic_sign_dataset/) for providing the data used in this project.
- The developers of OpenCV, TensorFlow, and Keras for their invaluable tools and libraries.
