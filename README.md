# Smart-FIR-Management-System
# 🚓 Smart-FIR Management System
> **A Next-Gen Police Incident Reporting Tool powered by NLP and Geolocation.**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Framework](https://img.shields.io/badge/Framework-Flask-green)
![ML](https://img.shields.io/badge/AI-Scikit--Learn-orange)
![Law](https://img.shields.io/badge/Law-BNS%20Compliant-red)

## 📖 Project Abstract
The **Smart-FIR Management System** is an AI-driven web application designed to modernize the First Information Report (FIR) process. By leveraging **Natural Language Processing (NLP)**, the system analyzes incident descriptions (via text or voice) and automatically recommends the relevant **Bharatiya Nyaya Sanhita (BNS)** section. This reduces human error, speeds up filing, and provides Headquarters with real-time geospatial crime analytics.

---

## 🌟 Key Features

### 👮 For Field Officers (User Mode)
* **AI Legal Assistant:** Uses **TF-IDF Vectorization** and **Cosine Similarity** to match incident descriptions against a legal database (e.g., Murder, Theft, Cheating, Rash Driving).
* **Voice-to-Text Reporting:** Integrated Web Speech API allows officers to dictate incidents hands-free.
* **Auto-Geolocation:** Automatically captures the officer's latitude and longitude to tag the precise crime scene.

### 🏢 For Headquarters (Admin Mode)
* **Live Command Dashboard:** visualizes total logged incidents and their statuses.
* **Interactive Crime Map:** Uses **Leaflet.js** to plot incident pins on a map, allowing admins to see crime hotspots.
* **Official PDF Generation:** One-click download of a formatted "Official Police Incident Log" using the `FPDF` library.

---

## 🛠️ Tech Stack

| Component | Technology Used |
| :--- | :--- |
| **Backend** | Python, Flask |
| **Machine Learning** | Scikit-Learn (TF-IDF, Cosine Similarity), NumPy |
| **Frontend** | HTML5, Bootstrap 5, FontAwesome |
| **Mapping** | Leaflet.js, OpenStreetMap |
| **Database** | JSON (Lightweight file-based storage) |
| **Reporting** | FPDF (PDF Generation) |

---

## ⚙️ Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/your-username/Smart-FIR-Management-System.git](https://github.com/your-username/Smart-FIR-Management-System.git)
    cd Smart-FIR-Management-System
    ```

2.  **Install Dependencies**
    [cite_start]Ensure you have the required libraries installed[cite: 1]:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Application**
    ```bash
    python app.py
    ```

4.  **Access the Portal**
    * Open your browser and navigate to: `http://127.0.0.1:5000`
    * **Home:** Select "Officer Login" or "HQ Admin".

---

## 🧠 How the AI Works
The system utilizes a **Content-Based Filtering** approach:
1.  **Knowledge Base:** The system is pre-trained on keywords related to BNS sections (e.g., "stabbed" -> BNS Sec 103, "snatching" -> BNS Sec 304).
2.  **Vectorization:** It converts the user's input text into numerical vectors using `TfidfVectorizer`.
3.  **Similarity Check:** It calculates the cosine angle between the input vector and the legal database vectors to find the best match.

---

## 📸 Screenshots
<img width="1370" height="744" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/c5646017-1a28-44dc-88f7-8a07156e2959" />
<img width="1752" height="776" alt="Screenshot (74)" src="https://github.com/user-attachments/assets/08212486-4d96-493f-8596-f19578cb347e" />

---

## 📜 Legal & Compliance
This project is updated to reflect the new **Bharatiya Nyaya Sanhita (BNS)** criminal code replacing the IPC. Current supported sections include:
* **BNS Section 103:** Murder
* **BNS Section 303:** Theft
* **BNS Section 281:** Rash Driving
* ...and more.

---

## 👥 Contributors
* **Ayush S** - *Lead Developer*

---
