Food Rating Prediction - Flask Web App
This project is a web application that predicts the rating of food items based on their nutritional information (Calories, Protein, Fat, and Sodium). 
It uses a machine learning model (saved as a .pkl file) for predictions, and the application is built using Flask.

Table of Contents:
  - Installation
  - Setup
  - Running the App
  - Project Structure
  - Dependencies

Installation : 

Step 1: Clone the Repository
Clone this repository to your local machine:
  - git clone https://github.com/your-repo/your-project.git
    
Step 2: Create and Activate a Virtual Environment
  1. Navigate to the project folder:
       - cd your-project-folder
  2. Create a virtual environment:
      - python -m venv flask
  3. Activate the virtual environment:
      - .\flask\Scripts\activate

Step 3: Install Required Dependencies
After activating the virtual environment, install the required Python packages:
  - pip install -r requirements.txt
If you don't have a requirements.txt file yet, here's what to include:
  - Flask
  - numpy
  - scikit-learn

Setup :
Step 1: Place the Trained Model
  - Make sure your trained model file best_model.pkl is in the same directory as your app.py file.

Step 2: Modify the app.py if Needed
  - If your best_model.pkl is stored in a different directory, update the path in your app.py file accordingly:
      - model_file_path = "path/to/your/best_model.pkl"

Running the App :
  - Ensure your virtual environment is activated.
  - Navigate to the folder where your app.py file is located.
  - Run the Flask app using this command:
    - python -m flask --app .\app.py run
    - By default, the application will be available at: http://127.0.0.1:5000/

Project Structure :

your-project-folder/
│
├── flask/
│   ├── Scripts/           # Virtual environment scripts
│   └── ...
│
├── static/
│   └── style.css          # CSS for the application
│
├── templates/
│   └── index.html         # HTML form for input
│
├── best_model.pkl          # Pre-trained machine learning model (ensure this is placed here)
├── app.py                  # Flask app code
├── requirements.txt        # List of dependencies
└── README.md               # This file

Dependencies :
  - Flask: For web application development
  - numpy: For numerical operations
  - scikit-learn: For loading the machine learning model


