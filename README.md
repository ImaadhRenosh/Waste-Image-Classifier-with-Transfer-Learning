# Waste-Image-Classifier-with-Transfer-Learning

## Table of Contents
- [Overview](#overview)
- [Aim of the Project](#aim-of-the-project)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation & How to Run](#installation--how-to-run)
- [Screenshots / Demo](#screenshots--demo)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Overview
EcoClean currently lacks an efficient and scalable method to automate the waste sorting process. The manual sorting of waste is not only labor-intensive but also prone to errors, leading to contamination of recyclable materials. The goal of this project is to leverage machine learning and computer vision to automate the classification of waste products, improving efficiency and reducing contamination rates. The project will use transfer learning with a pre-trained VGG16 model to classify images.

## Aim of the Project
The aim of the project is to develop an automated waste classification model that can accurately differentiate between recyclable and organic waste based on images. By the end of this project, you will have trained, fine-tuned, and evaluated a model using transfer learning, which can then be applied to real-world waste management processes.

## Technologies Used
- **Programming Language:** Python
- **Libraries:** TensorFlow, Keras, OpenCV
- **Tools:** Jupyter Notebook, Git, VS Code

## Prerequisites
- Python (version 3.6 or higher)
- Git
- Jupyter Notebook

## Installation & How to Run
To set up and run the project locally:

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/ImaadhRenosh/Waste-Image-Classifier-with-Transfer-Learning.git
    cd Waste-Image-Classifier-with-Transfer-Learning
    ```

2. **Install Dependencies**: Install the required libraries using:
    ```sh
    !pip install tensorflow==2.17.0 | tail -n 1
    !pip install numpy==1.24.3 | tail -n 1
    !pip install scikit-learn==1.5.1  | tail -n 1
    !pip install matplotlib==3.9.2  | tail -n 1
    ```

3. **Run the Jupyter Notebook**: Launch Jupyter Notebook and open `waste_classifier.ipynb` to train and evaluate the model.

## Screenshots / Demo

- **Screenshot 1/ Importing Required Libraries**:
<img width="716" alt="Screenshot 2025-03-15 at 05 59 51" src="https://github.com/user-attachments/assets/2d92812a-95c8-42fb-8414-e3040bcd0842" />

- **Screenshot 2/ Importing Data**:
<img width="1011" alt="Screenshot 2025-03-15 at 06 01 10" src="https://github.com/user-attachments/assets/7fabec08-c102-4b0f-a662-0ba234db9228" />

- **Screenshot 3/ Defining configuration options**:
<img width="456" alt="Screenshot 2025-03-15 at 06 02 25" src="https://github.com/user-attachments/assets/b194e7f8-a6fd-4aa0-8e43-67daa4f12589" />

- **Screenshot 4/ ImageDataGenerators**:
<img width="1084" alt="Screenshot 2025-03-15 at 06 03 29" src="https://github.com/user-attachments/assets/c7dc33eb-82cd-45c4-bc3a-90a44d8639d5" />
<img width="486" alt="Screenshot 2025-03-15 at 06 04 53" src="https://github.com/user-attachments/assets/d004efb8-70d2-4e30-9135-f0896ef4ea2c" />

- **Screenshot 5/ Step 1: Creating a test_generator using the test_datagen object**:
<img width="572" alt="Screenshot 2025-03-15 at 06 05 22" src="https://github.com/user-attachments/assets/99cb60dd-3ed2-466b-9e51-8a53e95b7e41" />

- **Screenshot 6/ Let's look at a few augmented images:**:
<img width="1014" alt="Screenshot 2025-03-15 at 06 07 29" src="https://github.com/user-attachments/assets/adc582ca-b0e0-41bd-abc0-8af0d7ea9771" />

- **Screenshot 7/ Pre-Trained Models / VGG-16**:
<img width="1022" alt="Screenshot 2025-03-15 at 06 08 26" src="https://github.com/user-attachments/assets/269b29d9-0141-444d-a5b7-311dcc10a673" />
<img width="951" alt="Screenshot 2025-03-15 at 06 32 05" src="https://github.com/user-attachments/assets/a4ee31a0-ad83-446d-8459-67e6e69cbcf4" />
<img width="689" alt="Screenshot 2025-03-15 at 06 32 33" src="https://github.com/user-attachments/assets/ca32f259-6ae5-4dcd-9503-23ee8c9f1693" />


- **Screenshot 9/ Step 2: Compile the Model**
<img width="501" alt="Screenshot 2025-03-15 at 06 33 16" src="https://github.com/user-attachments/assets/924db8fe-261e-45cc-ab2e-f258c14b8225" />

- **Model Summary**
<img width="806" alt="Screenshot 2025-03-15 at 06 35 07" src="https://github.com/user-attachments/assets/f6f99d4c-1d15-41e9-befb-d453aec28d5f" />

CallBack




## Usage
After launching the Jupyter Notebook, you can:
- Upload images of waste.
- The model will classify the waste as either recyclable or organic.

## Contributing
Contributions are welcome! If you’d like to improve this project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push the branch.
4. Open a pull request detailing your changes.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements
- Thanks to the contributors of TensorFlow, Keras, and OpenCV.
- Special thanks to the EcoClean team for their support and collaboration.

## Contact
For any questions or suggestions, feel free to reach out:
- **Email:** imaadhrenosh@gmail.com
- **LinkedIn profile**: [LinkedIn profile](https://www.linkedin.com/in/imaadh-renosh-007aba348)


