# 📚 Manage Books Library API  

A simple Django REST API project for managing a library system.  
Supports **CRUD** operations on books, members, and borrowing records with **JWT authentication**. 🚀  

## ✨ Features  

- ✅ **User authentication** with JWT (JSON Web Tokens)  
- ✅ **Manage Books** (Add, Edit, Delete, List) 📖  
- ✅ **Manage Members** (Add, Edit, Delete, List) 👥  
- ✅ **Manage Borrow Records** (Track borrowing and returning of books) 🔄  
- ✅ **API documentation** with Swagger and Redoc 📝  

## ⚙️ Requirements  

- 🔹 **Python 3.10+** 🐍  
- 🔹 **Django 5.1+** 🌍  
- 🔹 **Django REST Framework** 🛠  
- 🔹 **Simple JWT** for authentication 🔑  
- 🔹 **drf-yasg** for API documentation 📜  

## 🚀 Installation  

1️⃣ **Clone the repository:**  
```bash
git clone https://github.com/yourusername/library-management.git
cd library-management

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
3️⃣ Install dependencies:

pip install -r requirements.txt
4️⃣ Apply migrations:

python manage.py migrate
5️⃣ Create a superuser (optional, for admin access):

python manage.py createsuperuser
6️⃣ Run the development server:

python manage.py runserver
🎯 Usage
📌 Access API documentation:

Swagger UI: http://127.0.0.1:8000/swagger/

Redoc: http://127.0.0.1:8000/redoc/

🔑 Obtain JWT tokens: Send a POST request to /api/token/ with username and password to get Access and Refresh Tokens. Use the Access Token to authenticate API requests.

🔹 Available API endpoints for CRUD operations:

/api/books/

/api/members/

/api/borrows/

🛠 Testing
Run tests with:

bash
python manage.py test
📂 Project Structure
plaintext
pro/                 # Django project settings  
task/                # App containing models, views, serializers for the library system  
requirements.txt     # Python dependencies  
⚠️ Notes
🚨 This project uses SQLite by default. You can change the database settings in pro/settings.py. 🔒 Keep the SECRET_KEY safe in production environments! 🔹 For production, set DEBUG = False and configure Allowed Hosts.