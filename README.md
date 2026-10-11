# CampusConnect_DS — Data Science Platform

## 🛠️ How to Open and Run in VS Code

### Step 1: Open in VS Code
Open VS Code and choose **File ➔ Open Folder...**, then select:
`C:\Users\dhiraj12\Desktop\CampusConnect_DS`

### Step 2: Open Terminal in VS Code
Open the integrated terminal in VS Code (`Ctrl + ~` or **Terminal ➔ New Terminal**).

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Run Application
```bash
python app.py
```

### Step 5: Access the Web Portal
Open your web browser and navigate to:
**http://localhost:5000**

---

## 👥 Demo Login Credentials

| Role | College | Email | Password |
| :--- | :--- | :--- | :--- |
| **Student** | MCOE (Pune) | `rahul@ait.edu` | `student123` |
| **Student** | MCOE (Pune) | `priya@ait.edu` | `student123` |
| **Admin** | MCOE (Pune) | `admin@mcoe.edu.in` | `admin123` |
| **Admin** | Ferguson College | `admin@fc.edu.in` | `admin123` |
| **Admin** | VIT (Pune) | `admin@vit.edu.in` | `admin123` |

---

## 📁 Directory Structure
```
CampusConnect_DS/
├── .env                       # Environment configuration (read-only DB credentials)
├── requirements.txt           # Python dependencies (Flask, scikit-learn, pandas, pymysql)
├── config.py                  # Application configuration loader
├── database.py                # Read-only database query execution helper
├── auth.py                    # SHA-256 authentication & role decorators
├── partner_recommendation.py  # K-Means Study Partner Recommendation engine
├── event_recommendation.py    # TF-IDF Event Recommendation engine
├── lost_found_matching.py     # TF-IDF Lost & Found Matching engine
├── data_analysis.py           # Pandas EDA analytics & Chart.js data formatting
├── app.py                     # Flask web server and routing
├── templates/                 # Jinja2 HTML templates
│   ├── base.html              # Shared responsive navigation and layout
│   ├── login.html             # Secure login screen
│   ├── student_dashboard.html # Student portal overview
│   ├── partner.html           # Study Partner K-Means recommendation page
│   ├── events.html            # Event TF-IDF recommendation page
│   ├── lost_found.html        # Lost & Found similarity search & match page
│   ├── admin_dashboard.html   # Admin portal overview
│   ├── data_analysis.html     # Interactive Chart.js EDA dashboard
│   ├── admin_partners.html    # Admin student cluster inspection
│   └── admin_lost_found.html  # Admin lost & found matching report
└── static/
    ├── css/style.css          # CampusConnect styling theme
    └── js/main.js             # UI helpers
```
