# Image Captioning App with Pre-trained Model 📸

This project is an Image Captioning App built using Streamlit, PyTorch, and the BLIP (Bootstrapped Language-Image Pre-training) model from Salesforce. The app allows users to upload an image and generates multiple captions for the uploaded image.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model and Algorithm](#model-and-algorithm)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

The Image Captioning App is designed to provide an easy-to-use interface for generating captions for images. By leveraging the power of deep learning and the BLIP model, the app can generate descriptive captions that capture the essence of the uploaded images.

## Features

- Upload images in JPG, JPEG, or PNG format.
- Generate multiple captions for each uploaded image.
- User-friendly interface with a clean and modern design.
- GPU support for faster caption generation.

## Installation

To run the app locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/image-captioning-app.git
   cd image-captioning-app
   ```

2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## Usage

1. Open your web browser and navigate to the URL provided by Streamlit, typically `http://localhost:8501`.

2. Upload an image by clicking the "Choose an image..." button and selecting a file.

3. Wait for the app to generate captions. The generated captions will be displayed below the uploaded image.

## Model and Algorithm

### BLIP Model

The app uses the BLIP (Bootstrapped Language-Image Pre-training) model from Salesforce, which is designed for image captioning tasks. The model is capable of generating high-quality captions by leveraging pre-trained language and vision transformers.

### Algorithm

1. **Image Upload**: The user uploads an image using the Streamlit file uploader.
2. **Image Processing**: The uploaded image is processed and prepared for caption generation.
3. **Caption Generation**: The BLIP model generates multiple captions for the processed image using beam search with 5 beams and returns 3 captions.
4. **Display**: The app displays the uploaded image and the generated captions in a user-friendly interface.

## Project Structure

```plaintext
image-captioning-app/
├── app.py                # Main application file
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgements

- [Streamlit](https://streamlit.io/) for providing an easy-to-use web application framework.
- [Hugging Face](https://huggingface.co/) for providing the BLIP model.
- [Pillow](https://python-pillow.org/) for image processing.
