# Jels International Car Dealership 

This web application was developed as the final Capstone Project for the **IBM Full Stack / Cloud Developer Professional Certificate**. 


The platform acts as a centralized review portal for **Jels International**, a fictional nationwide car dealership network, allowing users to browse dealership locations by state, view localized reviews, and submit their own customer feedback.

The project showcases a modern, containerized microservices architecture combining Python (Django), JavaScript (React, Node.js), and cloud-native integrations.

---

## 🏗️ Architecture Overview

The system is split into loosely coupled microservices interacting via REST APIs:

1. **Jels International Frontend & Gateway (Django & React):**
2.
3. The central hub managing user authentication (SQLite), car makes/models catalog, and serving as the proxy layer to fetch data from backend microservices.
4.
5.  **Dealerships & Reviews Service (Node.js/Express):**
6.
7. Handles CRUD operations for Jels International dealer profiles and review records stored in a **MongoDB** instance.
8.
9.  **Sentiment Analyzer (Python Flask / IBM Watson NLU):**
10.
11.  Deployed on **IBM Cloud Code Engine**.
12.
13.  It processes raw user review text and classifies the sentiment into `positive`, `neutral`, or `negative`.

---

## 🛠️ Tech Stack

*   **Frontend:** React.js, Bootstrap 5, HTML5, CSS3
*   **Backend Framework:** Django (Python)
*   **Microservices:** Node.js, Express.js, Flask
*   **Databases:** SQLite (Auth & Car Inventory), MongoDB (Dealer Profiles & Reviews)
*   **Containerization & Cloud:** Docker, Docker Compose, IBM Cloud Code Engine, Kubernetes

---

## 🚀 Key Features

*   **Anonymous Browsing:** Filter and view all Jels International branches nationwide sorted by location and state.
*   **Authorized User Portal:** Secure user registration, login/logout sessions, and permission to submit new reviews for specific dealerships.
*   **AI Sentiment Analytics:** Every review automatically runs through the Sentiment Analyzer to display a corresponding mood icon (happy/neutral/sad face) next to user feedback.
*   **Microservice Deployment:** Complete containerization of background services for scalable cloud deployment.

---

## 💻 Setup & Installation Instructions

### Prerequisites
*   Python 3.10+
*   Node.js (v18+)
*   Docker & Docker Compose
*   An active IBM Cloud Account (for Code Engine / Watson NLU deployment)

---

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/jels-international-car-dealer.git](https://github.com/YOUR_USERNAME/jels-international-car-dealer.git)
cd jels-international-car-dealer
