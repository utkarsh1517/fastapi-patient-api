# fastapi-patient-api

A simple and functional FastAPI REST API to manage patient records using Pydantic models, validation, and computed fields(BMI + Health Verdict).

# Features  
- Add new patient  
- View all patients  
- View a specific patient  
- Update patient details  
- Delete patient  
- Auto-calculation of BMI  
- Auto-generated health verdict
- Sorting patients by height, weight, or BMI  
- Input validation using Pydantic
- Data stored in JSON file (file-based mini-database)

# Tech Stack  
- Python 3.10+ 
- FastAPI  
- Uvicorn  
- Pydantic v2

# Installation & Setup
1 Clone the repository
2 Install dependencies
3 Run the application
4 API Documentation  
  Once the server is running:
   Swagger UI: http://127.0.0.1:8000/docs 

# API Endpoints

➤ GET / 
Check API status.
➤ GET /view 
Get all patients.
➤ GET /patient/{patient_id}
Fetch a single patient by ID.
➤ POST /create  
Add a new patient.  
➤ PUT /edit/{patient_id}
Update patient details (partial update allowed).
➤ DELETE /delete/{patient_id}
Remove a patient.
➤ GET /sort?sort_by=bmi&order=desc
Sort patients by height/weight/BMI in ascending or descending order.

# Project Structure
fastapi-patient-api/
│── main.py
│── patient.json
│── requirements.txt
└── README.md

# License
This project is licensed under the MIT License.


