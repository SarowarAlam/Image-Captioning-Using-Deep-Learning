# BD Heritage Image Captioning Using Deep Learning

## Overview

This project focuses on using image captioning techniques to highlight the cultural heritage of Bangladesh. It employs cutting-edge deep learning models to generate accurate textual descriptions of images, aiming to promote Bangladeshi culture and heritage to a global audience. The system is particularly beneficial for travelers and educational purposes, ensuring wider recognition of the country's rich history and traditions.

---

## Key Features

- **Image Captioning**: Generates human-like captions for images of Bangladeshi cultural and heritage sites.
- **Web Interface**: A user-friendly Flask-based web application for image upload and caption prediction.
- **Translation Support**: Auto-generated captions can be translated into Bengali using Google Translator API.
- **Pre-trained Models**: Uses ResNet50 and LSTM networks for accurate image feature extraction and sequence prediction.
- **Custom Dataset**: Focused on Bangladeshi heritage, trained on 1,500 images with five captions per image from the Flickr8k dataset.

---

## Methodology

The project utilizes a hybrid deep learning approach with CNNs and LSTMs:
1. **Feature Extraction**: ResNet50 extracts features from images, leveraging its 50-layer architecture.
2. **Sequence Generation**: LSTM networks process extracted features to generate coherent and meaningful captions.
3. **Dataset Preparation**: Customized dataset of Bangladeshi heritage images, labeled with captions in five scenarios.
4. **Web Application**: Flask framework integrates the trained model with a web interface for real-time captioning.

---

## Technical Details

### Model Architecture
- **ResNet50**:
  - Pre-trained on ImageNet.
  - Extracts 2048-dimensional feature vectors from input images.
- **LSTM**:
  - Processes sequential data.
  - Includes mechanisms like forget gates to handle long-term dependencies.

### Tools and Libraries
- **Python**: Main programming language.
- **TensorFlow & Keras**: Deep learning framework for model training.
- **Flask**: Web framework for the application.
- **Google Translator API**: Supports caption translation to Bengali.

### Training
- Dataset: Flickr8k images labeled with captions specific to Bangladeshi heritage.
- Process:
  - Preprocess images to 224x224 pixels.
  - Train for 150 epochs using a combination of CNN and LSTM.
  - Achieved ~89% accuracy in generating meaningful captions.

---

## How It Works

1. **Upload Image**: The user uploads an image of a Bangladeshi heritage site.
2. **Generate Caption**: The system generates a caption using the trained model.
3. **Translate Caption**: Option to translate the caption into Bengali.
4. **Explore**: Users can explore the cultural and historical significance of the site through captions.

---

## Impact

This project addresses the global audience's lack of awareness about Bangladesh's cultural heritage by:
- Providing insightful descriptions of historical sites like Sundarban, Paharpur, and Cox's Bazar.
- Enhancing tourism and educational outreach for future generations.
- Creating an innovative AI application tailored for cultural promotion.

---

## Future Enhancements

- Extend the dataset to include more diverse images of Bangladesh.
- Improve translation capabilities by integrating additional language support.
- Optimize the model for faster caption generation.
- Integrate the system with mobile applications for broader accessibility.

---

## Setup and Installation

### Prerequisites
- Python 3.8+
- TensorFlow 2.x
- Flask
- Required Python libraries: `numpy`, `pandas`, `cv2`, `glob`, `matplotlib`

### Installation Steps
1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd <repo-name>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Flask application:
   ```bash
   python app.py
   ```
4. Access the web interface at `http://127.0.0.1:5000/`.

---

## Results

- Achieved ~89% captioning accuracy on the customized dataset.
- Web application demonstration:
  - **Caption Prediction**: Automatically generates captions for uploaded images.
  - **Translation**: Converts captions to Bengali for accessibility.

Sample output:

- Input Image:![image](https://github.com/user-attachments/assets/e1d2fafb-f24c-44ec-8f04-54a06f093d28)

- Predicted Caption: "Bangladeshi boy and a man taking their cow for bath"
- Translated Caption: ![image](https://github.com/user-attachments/assets/62b8759b-f942-45ee-9b9d-4485c1eddf87)


---

## Contributing

Contributions are welcome! Please fork this repository and submit pull requests with your improvements.

---

## Acknowledgments

Special thanks to the authors of the paper *"Image Captioning - Bangladesh’s Heritage Perspective Using Deep Learning"* for their foundational work and the datasets used in this project.

---

Feel free to adapt this draft as needed for your GitHub repository. Let me know if you need additional modifications!
