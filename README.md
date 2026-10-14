# CarePulse Health - Healthcare Management System (Full Stack)

A full-stack clinical healthcare and Electronic Health Records (EHR) management system built with **HTML5, CSS3, JavaScript, React, Node.js, Express, and MySQL**.

---

## 🌐 Live Local Links

| Component | URL | Description |
| :--- | :--- | :--- |
| **Frontend UI (React + Vite)** | [http://localhost:5173](http://localhost:5173) | Interactive Clinical Dashboard & EHR Portal |
| **Backend REST API (Node + Express)** | [http://localhost:5000/api](http://localhost:5000/api) | API Root & Endpoints |
| **Health & DB Status** | [http://localhost:5000/api/stats/health](http://localhost:5000/api/stats/health) | Live Health Check & DB Diagnostics |
| **Analytics API** | [http://localhost:5000/api/stats/dashboard](http://localhost:5000/api/stats/dashboard) | Hospital Metrics & Appointments |

---

## 🏥 Key Features

1. **Clinical Analytics Dashboard**:
   - Total patients, daily consultations, doctor roster, revenue tracking.
   - Department workload visualization.
   - Quick appointment status toggling (Confirm, Complete, Cancel).

2. **Patient Directory & EHR (Electronic Health Records)**:
   - Search by name, phone, email, and blood group filters.
   - Comprehensive EHR modals showing consultation histories, active prescriptions, and vitals.
   - Patient registration with demographics, chronic conditions, and allergy tracking.

3. **Specialist Doctor Directory**:
   - Filter by Department: Cardiology, Neurology, Pediatrics, Orthopedics, General Medicine, Dermatology.
   - Consultation fees, room allocations, experience, and direct scheduling.

4. **Appointment Scheduling**:
   - Calendar booking with patient selector, doctor assignment, time slots, and visit reasons.
   - Automated invoice generation linked to doctor consultation fees.

5. **Medical Records & Diagnoses**:
   - Detailed clinical documentation: symptoms, examination notes, lab/radiology orders, and treatment plans.

6. **Digital Pharmacy & Prescriptions (Rx)**:
   - Multi-drug prescription generator with dosage, frequency, duration, and instructions.
   - Clean printable prescription slip layout.

7. **Patient Vitals Tracker**:
   - Blood pressure, pulse, body temperature, SpO2 oxygen saturation, blood sugar, weight & height.

8. **Billing & Invoices**:
   - Financial ledger tracking settled and outstanding balances.
   - One-click payment collection.

---

## 🗄️ MySQL Database Setup

The backend comes equipped with dual-engine capability:
- **Default Standalone Mode**: Works immediately out-of-the-box with seed healthcare data without requiring MySQL to be pre-configured.
- **MySQL Mode**: To connect your local MySQL server (XAMPP / WAMP / MySQL Workbench):

1. Check or import the schema file:
   `backend/src/database/schema.sql`
2. Configure credentials in `backend/.env`:
   ```env
   PORT=5000
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=your_password
   DB_NAME=carepulse_db
   DB_PORT=3306
   ```
3. Restart backend server: `npm start` in the `backend` folder. The app automatically provisions tables and sample records.

---

## 🚀 Running the Project

From the project root:

```bash
# Start Backend API (Port 5000)
cd backend
node src/server.js

# Start Frontend Dev Server (Port 5173)
cd frontend
npm run dev
```
