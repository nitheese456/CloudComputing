##About the Project

This project is completed in a group of three students as part of the CSE 546 course. Elastic application that can automatically scale out and in on demand and cost-effectively by using the PaaS cloud.

####Code Strucutre
.
├── Dockerfile
├── Readme.md
├── encoding
├── entry.sh
├── handler.py
├── mapping
├── requirements.txt
├── student_data.json
└── workload.py

Overview:

Our cloud app will implement a smart classroom assistant for educators. This assistant takes videos from the user’s classroom, performs face recognition on the collected videos, looks up the recognized students in the database, and returns the relevant academic information of each student back to the user.

## Getting Started

- Dockerfile - This file contains the code to create docker image.
- handler.py - This file contains the lambda handler and logic for our application.
- encoding - This file contains encodings of all the students.
- entry.sh - Scripts that is requried for docker file to setup the lambda.
- Run workload.py to upload the test videos to input S3 bucket.

#### Team Members

1. Ravi Maddi - Worked on aws account, docker and aws resources setup and handling input events.
2. Nitheese Thirumoorthy - Worked on face recognition logic.
3. Sai Achyuth Vellineni - Worked on face recognition logic and fetching data from DDB and stroing the csv files to S3.

##### AWS Resources

- AWS Credentials are provided in the Excel file.

  INPUT_BUCKET = 'cse546-input-project2'
  OUTPUT_BUCKET = 'output-project2-cse546'
