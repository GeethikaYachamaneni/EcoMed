# EcoMed

EcoMed is a medicinal plant identification and disease detection system designed to assist users in recognizing medicinal plants and diagnosing plant diseases. The project leverages image classification techniques and a structured dataset to provide accurate results.

## Technologies Used
- **Frontend:** Streamlit (for UI)
- **Backend:** Python, TensorFlow (for image classification)
- **Database:** JSON files (for storing plant information and remedies)
- **Development Environment:** VS Code on Windows 11
- **Python Version:** 3.11.5 (added to the system PATH during installation)

## Project Structure
```
EcoMed/
│-- app.py  # Main application file
│-- classify.py  # Handles plant classification
│-- datasplit.py  # Splits dataset into training, validation, and test sets
│-- models/  # Directory for trained models
│-- images/  # Stores sample images
│-- data/  # Contains dataset files
│-- plant_info.json  # Information about medicinal plants
│-- remedies.json  # Remedies for plant diseases
│-- venv/  # Virtual environment directory
```

## Execution Process
### 1. Setup Virtual Environment
To ensure a controlled environment, create and activate a virtual environment:
```sh
python -m venv venv
venv\Scripts\activate  # For Windows
```

### 2. Install Dependencies
Install the required Python packages:
```sh
pip install streamlit tensorflow pillow numpy
```

### 3. Run the Application
Execute the Streamlit application:
```sh
streamlit run app.py
```

### 4. Using EcoMed
- **Medicinal Plant Identification:** Upload an image to identify medicinal plants and get their descriptions.
- **Plant Disease Classifier:** Upload a plant image to check for diseases and receive remedies.

## Dataset
The dataset consists of categorized images of medicinal plants and diseased plants, organized into structured directories. The `datasplit.py` script splits the dataset into training, validation, and test sets.

## Model
The model used for classification is stored in the `models/` directory and is loaded dynamically during execution.

## Notes
- Ensure that `models/cnn_model.keras` and `models/plant_disease_prediction_model.h5` exist in the correct directory.
- JSON files (`plant_info.json`, `remedies.json`) must be available for plant descriptions and remedies.
- If permission errors occur, run the terminal as an administrator.

🚀

