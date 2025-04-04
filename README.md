# Image Captioning and Translation Web App

## Overview
This project is a Flask-based web application that allows users to upload an image, generate a caption using a pre-trained image captioning model, and translate the caption into a selected language.

## Features
- **Image Upload:** Users can upload images in PNG, JPG, JPEG, or GIF formats.
- **Image Captioning:** Generates a caption for the uploaded image using the `nlpconnect/vit-gpt2-image-captioning` model.
- **Translation:** Translates the generated caption into the selected target language.
- **Display:** The uploaded image and translated caption are displayed on the webpage.

## Technologies Used
- **Backend:** Flask
- **Machine Learning Models:** Hugging Face Transformers (`nlpconnect/vit-gpt2-image-captioning`)
- **Libraries:**
  - `transformers`: For image captioning
  - `PIL` (Pillow): For image processing
  - `translate`: For text translation
  - `torch`: For deep learning model computations
  - `werkzeug.utils`: For file handling
  
## Installation
### Prerequisites
- Python installed (version 3.7 or later)
- `pip` installed

### Steps to Run the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/image-captioning.git
   cd image-captioning
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the Flask application:
   ```sh
   python app.py
   ```
4. Open `http://127.0.0.1:5000/` in your browser.

## Usage
1. Upload an image.
2. Select a target language for translation.
3. Click on the "Submit" button.
4. View the generated caption and translated text.

## Folder Structure
```
image-captioning/
│── static/
│   └── uploads/   # Folder where uploaded images are stored
│── templates/
│   └── cap.html   # HTML template for the web UI
│── app.py         # Flask application
│── caption.py     # Image captioning logic
│── requirements.txt  # Required dependencies
```

## Contribution
Feel free to fork the project, raise issues, and contribute to improvements.

## License
This project is licensed under the MIT License.
