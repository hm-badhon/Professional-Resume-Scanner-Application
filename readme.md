

# Professional Resume Scanner Application 

## Project Overview

This Flask application is designed to classify resumes into various job categories using a machine learning model. The application allows users to upload their resumes, which are then processed and classified into a predefined category using a trained model.

## Features

- **Resume Upload**: Users can upload resumes in text format.
- **Resume Cleaning**: The application preprocesses and cleans the resume text.
- **Resume Classification**: The cleaned text is classified into one of the predefined job categories.
- **User-Friendly Interface**: The application features a simple and modern web interface for ease of use.

## Requirements

- Python 3.x
- Flask
- scikit-learn
- nltk

## Installation

1. **Clone the Repository**

```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
```

2. **Set Up a Virtual Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

   If `requirements.txt` is not available, you can manually install the necessary packages:

   ```bash
   pip install flask scikit-learn nltk
   ```

4. **Download NLTK Data**

   Ensure you have the necessary NLTK data:

   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

5. **Download or Train Models**

   Ensure you have the pre-trained models `clf.pkl` and `tfidf.pkl`. Place these files in the root directory of your project.

## Usage

1. **Run the Flask Application**

   ```bash
   python app.py
   ```

   The application will start and be accessible at `http://127.0.0.1:5000`.

2. **Access the Application**

   Open a web browser and navigate to `http://127.0.0.1:5000`. You will see a form to upload resumes.

3. **Upload a Resume**

   Use the form to upload a resume file. The application will process the resume and display the predicted job category.

## Project Structure

```
your_project/
│
├── static/
│   └── style.css       # CSS file for styling
│
├── templates/
│   └── index.html       # HTML template for the main page
│
├── app.py              # Main application file
├── clf.pkl             # Trained model for classification
├── tfidf.pkl           # Trained TF-IDF vectorizer
├── requirements.txt    # List of required Python packages
└── README.md           # This file
```

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. Make sure to follow the coding style and include tests for your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Flask**: A micro web framework for Python.
- **scikit-learn**: A machine learning library for Python.
- **nltk**: A library for natural language processing.


