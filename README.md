HEALTHCARE INDUSTRY DATA ANALYSIS
This project is a full-stack data collection and analysis system developed using Flask, MongoDB, and pandas.
The goal is to collect survey data on participants’ income and spending habits and analyze patterns to support decision-making for a healthcare product launch.
The system includes:
•	A web-based survey form
•	A MongoDB database for storage
•	A data processing pipeline using pandas
•	Visualizations for business insights
Technologies Used
•	Backend: Python (Flask)
•	Database: MongoDB
•	Data Processing: pandas
•	Visualization: matplotlib, seaborn
•	Frontend: HTML (Flask templates)
•	Deployment: AWS (EC2 / Elastic Beanstalk)
Project Structure
survey-app/
│
├── app.py                 # Flask application
├── templates/
│   └── index.html        # Survey form
├── models/
│   └── user.py           # User class
├── data/
│   └── users.csv         # Exported dataset
├── notebook/
│   └── analysis.ipynb    # Data analysis & visualization
├── requirements.txt
└── README.md

Features
•	Collects user data:
o	Age
o	Gender
o	Total Income
o	Expense categories:
	Utilities
	Entertainment
	School Fees
	Shopping
	Healthcare
•	Stores responses in MongoDB
•	Exports data to CSV
•	Performs analysis using pandas
•	Generates visualizations for reporting
Analysis Performed:
•	Income by Age
•	Spending patterns by Gender
•	Category-based expense analysis
Deployment on AWS
Option 1: EC2
•	Launch Ubuntu instance
•	Install dependencies
•	Run
Option 2: Elastic Beanstalk
pip install awsebcli
eb init
eb create survey-env
eb deploy
Challenges & Learnings
•	Integrating Flask with MongoDB
•	Handling form data and validation
•	Transforming NoSQL data into structured CSV
•	Using pandas for real-world data analysis
•	Creating meaningful visualizations for stakeholders

