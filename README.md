# 📘 Campus Hiring Management (CHM)

Campus Hiring Management (CHM) is a full-stack Django-based web platform that simplifies college placement activities.  
It enables **students, TPOs (Training & Placement Officers), and recruiters** to manage the entire hiring workflow from a centralized system.

---

## 🚀 Overview

This system digitizes the campus recruitment process by providing:

- Student registration & eligibility checks  
- TPO-driven job posting & approval workflows  
- Application tracking & selection results  
- Admin dashboard for managing the hiring cycle  

The application is built with scalable Django architecture and clean UI using HTML, CSS, Bootstrap.

---

## 🏗️ Tech Stack

- **Backend:** Django, Python  
- **Frontend:** HTML, CSS, Bootstrap, JavaScript  
- **Database:** MySQL / SQLite  
- **Tools:** Git, GitHub  

---

## 🔧 Features

### 👨‍🎓 Student Features
- Register & create profile  
- Upload resume  
- View active company drives  
- Apply for job openings  
- Track application status (Applied → Shortlisted → Selected/Rejected)

### 🏫 TPO/Admin Features
- Admin login (secured)  
- Create, update, delete job postings  
- Approve or reject applications  
- Manage student database  
- Publish shortlisted & final selected candidates  
- Dashboard showing hiring insights  

### 🏢 Recruiter (Optional)
- Add job descriptions  
- Access eligible student lists  

---

## 📁 Project Structure

Campus_Hiring/
│── manage.py
│── db.sqlite3
│── README.md
│
├── chm/ # Django project settings
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
│
├── app/ # Main application
│ ├── views.py
│ ├── models.py
│ ├── urls.py
│ ├── forms.py
│ └── admin.py
│
├── templates/ # HTML templates
│ ├── login.html
│ ├── register.html
│ ├── dashboard.html
│ └── apply_job.html
│
└── static/ # CSS, JS, images
├── css/
├── js/
└── images/


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/CHM.git
cd CHM

2️⃣ Create & activate virtual environment
python -m venv venv
venv\Scripts\activate    # Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Apply migrations
python manage.py migrate

5️⃣ Create admin user
python manage.py createsuperuser

6️⃣ Run server
python manage.py runserver

🔗 User Roles
Role	Access
Student	Register & apply for jobs
TPO/Admin	Full system management
Recruiter (optional)	Can post jobs
