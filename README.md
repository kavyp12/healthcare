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
   npm install 
   ```
2. Set up environment variables:
```bash
 echo "PROJECT_ID=" >> .env.local && \
   echo "API_KEY=" >> .env.local && \
   echo "DATABASE_ID=" >> .env.local && \
   echo "PATIENT_COLLECTION_ID=" >> .env.local && \
   echo "DOCTOR_COLLECTION_ID=" >> .env.local && \
   echo "APPOINTMENT_COLLECTION_ID=" >> .env.local && \
   echo "NEXT_PUBLIC_BUCKET_ID=" >> .env.local && \
   echo "NEXT_PUBLIC_ENDPOINT=https://cloud.appwrite.io/v1" >> .env.loca
```
  
3.Run the development server:
```bash
npm run dev
```


## Usage
Patient: Register or log in to book an appointment.
Admin: Approve or cancel appointments based on doctor availability. Notifications will be sent to patients via SMS.

