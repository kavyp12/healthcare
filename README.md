# Healthcare Appointment System

This project is a web-based hospital appointment system that allows patients to schedule appointments, and administrators to manage them. Notifications for appointment approvals or cancellations are sent via SMS using Twilio.

## Features

- Patient registration and login
- Appointment scheduling
- Admin approval and cancellation of appointments
- SMS notifications for patients
- User authentication and validation

## Tech Stack

- **Frontend**: Next.js, JavaScript, TypeScript
- **Backend**: Appwrite (Database)
- **SMS Notifications**: Twilio
- **Environment Variables**: Managed using `env.local`

## Installation

To set up the project locally, follow these steps:

1. Clone the repository, navigate to the directory, install dependencies, and set up the environment variables—all in one go:
   
   ```bash
   git clone https://github.com/kavyp12/healthcare.git && \
   cd healthcare && \
   npm install && \
   echo "PROJECT_ID=66a366ef000c23b29375" >> .env.local && \
   echo "API_KEY=42a4cfc422252fd5f427c0ef612d9b58e7f2a9c29509ada99cae8a599468dcae46289af0faae99cd9607d2b11aa25af4b3b109d55a26f43ceacb0311df9ec231536d50decc38fdc1f313f46f33221daabee492cb4168b7dc077da60c7d094c5429f0eed6d96f5ab34deebb210a624eece268a220ddd8f0d28b50e72f72ddf0e9" >> .env.local && \
   echo "DATABASE_ID=" >> .env.local && \
   echo "PATIENT_COLLECTION_ID=" >> .env.local && \
   echo "DOCTOR_COLLECTION_ID=" >> .env.local && \
   echo "APPOINTMENT_COLLECTION_ID=" >> .env.local && \
   echo "NEXT_PUBLIC_BUCKET_ID=" >> .env.local && \
   echo "NEXT_PUBLIC_ENDPOINT=https://cloud.appwrite.io/v1" >> .env.local && \
   echo "NEXT_PUBLIC_ADMIN_PASSKEY=123456" >> .env.local


2.Run the development server:
```bash
npm run dev
```


## Usage
Patient: Register or log in to book an appointment.
Admin: Approve or cancel appointments based on doctor availability. Notifications will be sent to patients via SMS.

## Environment Variables
The .env.local file should contain the following variables:

PROJECT_ID: Your Appwrite Project ID.
API_KEY: Your Appwrite API Key.
DATABASE_ID: Your Appwrite Database ID.
PATIENT_COLLECTION_ID: ID for the patient collection in Appwrite.
DOCTOR_COLLECTION_ID: ID for the doctor collection in Appwrite.
APPOINTMENT_COLLECTION_ID: ID for the appointment collection in Appwrite.
NEXT_PUBLIC_BUCKET_ID: Your Appwrite bucket ID.
NEXT_PUBLIC_ENDPOINT: The Appwrite endpoint for your database.
NEXT_PUBLIC_ADMIN_PASSKEY: The passkey for admin access.


