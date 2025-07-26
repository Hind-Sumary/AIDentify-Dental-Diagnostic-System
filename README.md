# AIDentify - Dental Diagnostic System

This repository contains the source code for AIDentify, a dental diagnostic system designed as a decision support tool for dentists. This web-based application streamlines the process of dental image analysis, diagnosis, and reporting, offering a comprehensive solution for dental professionals.




## Features

AIDentify caters to three distinct user roles: Admin, Doctor, and Employee, each with tailored functionalities to ensure efficient workflow and secure data management.

### Admin Features

Admins have overarching control over user management and system monitoring:

- **User Management:** Admins can review and accept applications from new users, manage existing user roles (e.g., changing a user's role from Employee to Doctor), and deactivate users as needed.

![Role Management Admin](/Images/roleManagementAdmin.jpeg)

- **Admin Addition:** Ability to add new administrators to the system.
- **System Logs:** Access to a detailed log file that tracks user activities within the system for security and auditing purposes.

![Log Display for Admin](/Images/logDisplayForAdmin.jpeg)

### Doctor Features

Doctors are equipped with advanced tools for dental image analysis and patient report generation:

- **Image Upload & Enhancement:** Upload dental X-ray images and enhance them using the CLHE (Contrast Limited Adaptive Histogram Equalization) algorithm.

![Main Screen Doctor](/Images/mainScreenDoctor.jpeg)

![Enhancement Screen](/Images/Enhancment.jpeg)

- **Dual Model Analysis:**
    - **Model 1 (Scratch-built):** Analyzes images for four types of diagnoses (e.g., ectopic, caries, Decayed teeth) and identifies healthy teeth. The diagnosis appears with a confidence level.
    - **Model 2 (Pre-trained):** Performs image segmentation and colorization, visually displaying annotations and diagnostics on the X-ray image. This model is based on a pre-trained model.d
- **Image Navigation & Inversion:** Doctors can navigate through uploaded images and invert them for medical examination purposes.
- **Checklist-based Diagnosis:** Diagnosis results from both models are presented in a checklist format, allowing doctors to confirm and select the correct findings.
- **Report Generation:** Generate comprehensive PDF reports for patients, including patient data and diagnostic findings. These reports are directly accessible from the doctor's page and the reports section.
  
![Report Management Doctor & Employee](/Images/reportManagementDoctor&Employee.jpeg)

- **Statistics & Research:** Access to statistical screens displaying diagnostic trends in bar graph form, categorized by model version (v1 or v2), useful for research and analysis.

![Statistics Screen](/Images/statisticsScreen.jpeg)

- **Recent Analyses:** View a history of recent analyses performed, including scan ID, doctor, diagnosis result, and date.

![Recent Analysis Screen](/Images/RecentAnalysisScreen.jpeg)

### Employee Features

Employees primarily assist with report management and communication:

- **Report Navigation:** Access and navigate through patient reports.
- **Email Report:** Send patient reports via email directly from the clinic to the patient.




## Storage

All photos, reports, and log data are securely stored in an S3 bucket using Amazon Web Services (AWS), ensuring data integrity and security.

## Training and Feedback

AIDentify is designed to be user-friendly and easy to train on. It has been deployed in multiple clinics for testing and feedback collection, enabling continuous improvement and refinement of the system.




## Demo Video

<video src="(https://github.com/user-attachments/assets/ec640cb5-0e55-451a-b21c-f4f230e24cfb)" controls width="600"></video>


## Team

- @Hind-Sumary
- @batoolShene
- @ali-m-keishe
