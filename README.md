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
EcoClean currently lacks an efficient and scalable method to automate the waste sorting process. The manual sorting of waste is not only labor-intensive but also prone to errors, leading to contamination and inefficient recycling. To address these issues, I have developed this project to use transfer learning and image classification to automate waste sorting.

## Aim of the Project
The aim of this project is to develop an automated waste classification model that can accurately differentiate between recyclable and organic waste based on images. By the end of this project, I aim to provide a robust solution to improve the efficiency and accuracy of the waste sorting process.

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

- Importing Required Libraries**:
<img width="716" alt="Screenshot 2025-03-15 at 05 59 51" src="https://github.com/user-attachments/assets/2d92812a-95c8-42fb-8414-e3040bcd0842" />


- Importing Data**:
<img width="1011" alt="Screenshot 2025-03-15 at 06 01 10" src="https://github.com/user-attachments/assets/7fabec08-c102-4b0f-a662-0ba234db9228" />


- **Defining configuration options**:
<img width="456" alt="Screenshot 2025-03-15 at 06 02 25" src="https://github.com/user-attachments/assets/b194e7f8-a6fd-4aa0-8e43-67daa4f12589" />


- **ImageDataGenerators**:
<img width="1084" alt="Screenshot 2025-03-15 at 06 03 29" src="https://github.com/user-attachments/assets/c7dc33eb-82cd-45c4-bc3a-90a44d8639d5" />
<img width="486" alt="Screenshot 2025-03-15 at 06 04 53" src="https://github.com/user-attachments/assets/d004efb8-70d2-4e30-9135-f0896ef4ea2c" />


- **Step 1: Creating a test_generator using the test_datagen object**:
<img width="572" alt="Screenshot 2025-03-15 at 06 05 22" src="https://github.com/user-attachments/assets/99cb60dd-3ed2-466b-9e51-8a53e95b7e41" />


- **Let's look at a few augmented images**::
<img width="1014" alt="Screenshot 2025-03-15 at 06 07 29" src="https://github.com/user-attachments/assets/adc582ca-b0e0-41bd-abc0-8af0d7ea9771" />


- **Pre-Trained Models / VGG-16**:
<img width="1022" alt="Screenshot 2025-03-15 at 06 08 26" src="https://github.com/user-attachments/assets/269b29d9-0141-444d-a5b7-311dcc10a673" />
<img width="951" alt="Screenshot 2025-03-15 at 06 32 05" src="https://github.com/user-attachments/assets/a4ee31a0-ad83-446d-8459-67e6e69cbcf4" />


- **Model Summary**:
<img width="689" alt="Screenshot 2025-03-15 at 06 32 33" src="https://github.com/user-attachments/assets/ca32f259-6ae5-4dcd-9503-23ee8c9f1693" />


- **Step 2: Compile the Model**:
<img width="501" alt="Screenshot 2025-03-15 at 06 33 16" src="https://github.com/user-attachments/assets/924db8fe-261e-45cc-ab2e-f258c14b8225" />


- **Callback function with Learning Rate Scheduler**
<img width="806" alt="Screenshot 2025-03-15 at 06 35 07" src="https://github.com/user-attachments/assets/f6f99d4c-1d15-41e9-befb-d453aec28d5f" />


- **Step 3: Fit and train the model**
<img width="1028" alt="Screenshot 2025-03-15 at 06 49 42" src="https://github.com/user-attachments/assets/b2fd1329-3ff3-485c-ac2f-7f293d3484a7" />


- **Step 4: Plot loss curves for training and validation sets (extract_feat_model)**
<img width="705" alt="Screenshot 2025-03-15 at 06 51 15" src="https://github.com/user-attachments/assets/080ee93c-7466-44ad-987d-866f935c2560" />
<img width="471" alt="Screenshot 2025-03-15 at 06 58 59" src="https://github.com/user-attachments/assets/8b72f4ee-ed56-4b68-bf89-fd571a471839" />


- **Step 5: Plot accuracy curves for training and validation sets (extract_feat_model)**
<img width="565" alt="Screenshot 2025-03-15 at 07 00 48" src="https://github.com/user-attachments/assets/2770f1ce-fab5-41df-ab10-b47b1e8d65d7" />
<img width="539" alt="Screenshot 2025-03-15 at 07 01 07" src="https://github.com/user-attachments/assets/cbafe59d-9350-44ce-93cc-38f9eb519322" />


- **Step 6: Fine-Tuning model**:
Let's fine-tune the model by adjusting the relevant parameters.
<img width="417" alt="Screenshot 2025-03-15 at 07 39 03" src="https://github.com/user-attachments/assets/f1e073b9-cfab-46e3-b15b-ff9a4107fd2b" />

- **Similar to what was done before, I will create a new model on top, and add a Dropout layer for regularization**
<img width="735" alt="Screenshot 2025-03-15 at 07 40 14" src="https://github.com/user-attachments/assets/ed1fdea9-229f-46e9-a7c9-20b622c14f00" />
<img width="1015" alt="Screenshot 2025-03-15 at 07 40 49" src="https://github.com/user-attachments/assets/a6e4f0e0-f226-4fc5-88fc-f79b1383dd12" />


- **Step 7: Plot loss curves for training and validation sets (fine-tune model)**
<img width="571" alt="Screenshot 2025-03-15 at 07 41 52" src="https://github.com/user-attachments/assets/5728a2ea-8694-44cc-aad3-fd3c9d0cb4a6" />
<img width="506" alt="Screenshot 2025-03-15 at 07 42 19" src="https://github.com/user-attachments/assets/53cd076a-d398-46a4-ae65-40cfb739bdfd" />



- **Step 8: Plot accuracy curves for training and validation sets (fine tune model)**
<img width="666" alt="Screenshot 2025-03-15 at 07 44 15" src="https://github.com/user-attachments/assets/94e9abff-7316-4271-96b7-a0c75407e874" />
<img width="541" alt="Screenshot 2025-03-15 at 07 44 32" src="https://github.com/user-attachments/assets/5e426a7c-4eef-4a40-9b71-b43a27258019" />


- **Step 9: Evaluate both models on test data**

<img width="1044" alt="Screenshot 2025-03-15 at 07 50 50" src="https://github.com/user-attachments/assets/a05a1720-63d7-4538-84a5-108e61f95a09" />
<img width="716" alt="Screenshot 2025-03-15 at 07 51 18" src="https://github.com/user-attachments/assets/dd026f3a-3137-4e21-9cf1-e28130ffa642" />



<img width="739" alt="Screenshot 2025-03-15 at 07 52 43" src="https://github.com/user-attachments/assets/ac1bec91-83c9-4594-b847-1c7c5c9a53a2" />


- **Step 10: Plot a test image using Extract Features Model (index_to_plot = 1)**

<img width="1006" alt="Screenshot 2025-03-15 at 07 54 21" src="https://github.com/user-attachments/assets/af8f4772-7737-42c5-9837-9d3c4101b260" />
<img width="484" alt="Screenshot 2025-03-15 at 07 54 46" src="https://github.com/user-attachments/assets/599779a2-13bf-4677-b476-2f55aeb4bc1b" />



- **Step 11: Plot a test image using Fine-Tuned Model (index_to_plot = 1)**
<img width="1005" alt="Screenshot 2025-03-15 at 07 55 58" src="https://github.com/user-attachments/assets/bca84ab8-264b-4b34-82fc-20c6b84411b8" />
<img width="580" alt="Screenshot 2025-03-15 at 07 56 19" src="https://github.com/user-attachments/assets/65d43694-01d6-4680-b044-28e862d7b219" />



<img width="397" alt="Screenshot 2025-03-15 at 07 56 41" src="https://github.com/user-attachments/assets/dc771448-ac2c-4248-b634-da3b82b69cb8" />

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
This project is licensed under © IBM Corporation. All rights reserved.

## Acknowledgements
- Thanks to the contributors of TensorFlow, Keras, and OpenCV.
- Special thanks to the EcoClean team for their support and collaboration.

## Contact
For any questions or suggestions, feel free to reach out:
- **Email:** imaadhrenosh@gmail.com
- **LinkedIn profile**: [LinkedIn profile](https://www.linkedin.com/in/imaadh-renosh-007aba348)


