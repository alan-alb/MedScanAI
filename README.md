# Medical Image Classification and Disease Detection

## Introduction

In the rapidly evolving field of medical imaging, the application of deep learning techniques has brought about a transformative shift. This project aims to leverage deep learning models to classify and detect diseases from medical images. The system covers areas such as brain tumor detection, skin lesion classification, lung disease classification, and bone fracture detection. By integrating multiple specialized models, we seek to develop a robust and comprehensive system for automated medical image analysis.

## Features

- Upload medical images for analysis.
- Classify the type of scan: Brain, Skin, Lungs, or Bones.
- Detect specific diseases based on the scan type.
- View results on an intuitive web interface.
- Chat functionality powered by Google Generative Language API.

## Technology Stack

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS
- **Machine Learning**: TensorFlow, PyTorch, YOLO
- **Database**: SQLite
- **APIs**: Google Generative Language API

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/alan-alb/medical-image-classification.git
    ```
2. Navigate to the project directory:
    ```sh
    cd medical-image-classification
    ```
3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Set up the database:
    ```sh
    python manage.py migrate
    ```

5. Run the development server:
    ```sh
    python manage.py runserver
    ```

6. Open your web browser and navigate to `http://127.0.0.1:8000/`.

## Usage

1. **Upload Image**: On the home page, upload the medical image you want to analyze.
2. **View Results**: After uploading, the system will classify the image type and predict the disease. Results will be displayed on a new page.
3. **Chat Functionality**: Use the chat feature to interact with the system for further queries.

## Project Structure

- `views.py`: Contains the main logic for handling requests and responses.
- `urls.py`: Defines the URL routes for the application.
- `models.py`: Defines the database models.
- `mlmodels.py`: Contains the machine learning models and prediction functions.
- `templates/`: Directory containing HTML templates for the web interface.
- `static/`: Directory for static files like CSS and images.

## Model Details

- **Brain Tumor Detection**: Uses a CNN model to detect brain tumors from MRI scans.
- **Skin Lesion Classification**: Classifies various types of skin lesions using a deep learning model.
- **Lung Disease Classification**: Identifies diseases such as pneumonia and tuberculosis from chest X-rays.
- **Bone Fracture Detection**: Detects fractures from radiographic images using YOLO.

## Data Sources

- Brain Tumor Detection: Publicly available MRI image datasets.
- Skin Lesion Classification: Dermoscopic image datasets like ISIC.
- Lung Disease Classification: Chest X-ray datasets like ChestX-ray8.
- Bone Fracture Detection: Radiographic image datasets.

## Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) for more details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References

- "Effective CNNs for Brain Tumor Detection," Journal of Medical Imaging, 2020.
- "Deep Learning Models for Skin Lesion Classification," International Dermatology Journal, 2021.
- "Machine Learning in Lung Disease Identification," Respiratory Medicine Journal, 2019.
- "AI for Bone Fracture Detection," Orthopedic Imaging Review, 2022.

## Contact

For any inquiries or issues, please contact Alan Albuquerque at [your-email@example.com].
