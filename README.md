# ✈️ CONTRAIL COURT – Aircraft Trail Investigation System

## 📌 About the Project

CONTRAIL COURT is a web-based aircraft trail investigation system developed using the MERN stack. It helps investigators record and manage aircraft details, atmospheric conditions, contrail observations, supporting evidence, and investigation results in one place.

The system integrates live aircraft information from OpenSky and atmospheric data from Open-Meteo to provide additional context for investigations.

## 🎯 Objectives

* Collect and manage aircraft and flight information.
* Retrieve live aircraft data and atmospheric conditions.
* Record contrail observations and supporting evidence.
* Assess investigation priority using rule-based risk assessment.
* Track investigation status and maintain case records.
* Display investigation statistics through a dashboard.
* Generate downloadable investigation reports.

## ✨ Key Features

* **User Authentication:** Login and registration with protected access.
* **Dashboard:** View investigation statistics and recent cases.
* **Live Data Assistant:** Retrieve aircraft and atmospheric data using latitude and longitude.
* **Investigation Management:** Create, view, update, search, filter, and manage investigations.
* **Contrail Observation:** Record contrail type, persistence, and observation details.
* **Evidence Management:** Store supporting evidence descriptions and image references.
* **Risk Assessment:** Categorize cases into Low, Medium, and High priority using predefined rules.
* **Investigation Tracking:** Track cases through their investigation statuses.
* **E-Report Generation:** Generate downloadable PDF investigation reports.
* **Role-Based Access:** Provide different permissions for Admin and Investigator roles.

## 🛠️ Technologies Used

### Frontend

* React.js
* JavaScript
* HTML5
* CSS3
* Axios
* React Router

### Backend

* Node.js
* Express.js
* REST API
* JSON Web Token (JWT)

### Database

* MongoDB
* Mongoose

### External APIs

* **OpenSky Network API:** Provides aircraft state information.
* **Open-Meteo API:** Provides weather and atmospheric data.

## 🔄 System Workflow

1. The user logs into the system.
2. The dashboard displays investigation statistics.
3. The investigator creates a new investigation.
4. Flight details and location coordinates are entered.
5. Live aircraft and atmospheric data are retrieved when available.
6. Contrail observations and supporting evidence are recorded.
7. The system assigns a risk priority using predefined rules.
8. The investigator updates the case status and records the result.
9. An E-Report can be generated for documentation.

## 📊 Risk Assessment

The system uses predefined rules to classify investigations into three priority levels:

* **Low:** Lower investigation priority.
* **Medium:** Requires further review.
* **High:** Higher investigation priority.

These categories help organize investigation work. They are not official scientific hazard ratings or proof that an aircraft or contrail is dangerous.

## 📁 Project Structure

```text
CONTRAIL-COURT/
├── backend/
│   ├── index.js
│   ├── models.js
│   ├── middleware.js
│   ├── routes.js
│   └── .env
│
└── frontend/
    ├── src/
    │   ├── App.jsx
    │   ├── App.css
    │   ├── index.css
    │   ├── main.jsx
    │   └── api.js
    ├── index.html
    └── package.json
```

## ⚙️ Installation and Setup

### Prerequisites

* Node.js and npm
* MongoDB running locally or a MongoDB connection URI
* A modern web browser

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd CONTRAIL-COURT
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your repository URL.

### 2. Configure the Backend

```bash
cd backend
npm install
```

Create a `.env` file inside the backend folder:

```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/contrail_court
JWT_SECRET=replace_with_a_secure_secret
```

Make sure MongoDB is running before starting the backend.

Start the server:

```bash
node index.js
```

The backend should run at:

`http://localhost:5000`

### 3. Configure the Frontend

Open a second terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL displayed by Vite in your terminal, usually:

`http://localhost:5173`

## 🔐 User Roles

* **Admin:** Access to investigation management and authorized administrative actions, including investigation deletion.
* **Investigator:** Access to investigation workflows and case information according to assigned permissions.

## 🌍 Project Scope

CONTRAIL COURT provides a centralized platform for documenting and organizing aircraft-trail investigations. It combines aircraft information, atmospheric context, observations, and evidence to support investigation tracking and reporting.

The application is a case-management and decision-support system; it does not independently prove contrail hazards or calculate actual climate impact.



## 👩‍💻 Project Information

**Project Name:** CONTRAIL COURT – Aircraft Trail Investigation System
**Project Type:** MERN Stack Web Application
**Domain:** Aircraft Trail Investigation and Case Management

---

*Developed as an academic project to explore full-stack web development, external API integration, investigation workflows, and data-driven case management.*
