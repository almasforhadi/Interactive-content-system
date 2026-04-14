# 📚 Interactive Learning Platform

An interactive content-based learning platform built with Django that allows users to create, explore, and engage with rich educational content enhanced by highlights, multimedia explanations, and user reviews.

---

## 🚀 Features

### 👤 Authentication System

* User Registration & Login
* Profile Update
* Password Change (without logout)
* Secure authentication using Django built-in system

### 📝 Content Management

* Create rich content using CKEditor
* Organize content by Category & Subcategory
* Dynamic word highlighting system

### 🎯 Interactive Highlights

* Clickable highlighted words
* AJAX-based explanation loading
* Supports:

  * 📝 Text
  * 🖼 Image
  * 🎧 Audio
  * 🎥 Video
  * ▶️ YouTube Embed

### ⭐ Review System

* Add reviews to content
* Rating system (1–5)
* Input validation

### 🎨 UI/UX

* Responsive design using Bootstrap 5
* Clean and modern interface
* Modal-based explanation display

---

## 🛠 Tech Stack

* **Backend:** Django 6
* **Frontend:** HTML, Bootstrap 5, JavaScript
* **Database:** PostgreSQL
* **Rich Text Editor:** CKEditor
* **Forms:** Django Crispy Forms

---

## 📂 Project Structure

```
interactive_platform/
│
├── app/                # Main content app
├── accounts/           # Authentication app
├── templates/          # HTML templates
├── static/             # CSS, JS files
├── media/              # Uploaded media files
├── manage.py              
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/interactive-platform.git
cd interactive-platform
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Setup Environment Variables

Create a `.env` file:

```env
SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3
```

### 5️⃣ Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6️⃣ Create Superuser

```bash
python manage.py createsuperuser
```

### 7️⃣ Run Server

```bash
python manage.py runserver
```

Visit:

```
http://127.0.0.1:8000/
```

---

## 🔑 Key Functionalities

### 🔹 Highlight System

* Words stored in database
* Dynamically highlighted using regex
* Click event triggers AJAX request to fetch explanation

### 🔹 Explanation System

Each highlight supports:

* Text
* Image
* Audio
* Video
* YouTube embed link

### 🔹 Review System

* Users can submit reviews
* Rating validation (1–5)
* Prevents empty submissions

---

## 🔐 Security

* Environment variables used for sensitive data
* CSRF protection enabled
* Login required for content creation

---

## 📌 Future Improvements

* Search & filtering system
* User roles (Admin / Editor)
* Bookmark & Like feature
* REST API integration (Django REST Framework)
* Pagination

---

## 👨‍💻 Author

<i>Almas Forhadi</i></br>
Django Developer

---

## 📄 License

This project is developed for educational and job assessment purposes.
