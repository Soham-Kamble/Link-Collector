# 🔗 Django Link Collector / Web Scraper

This is a Django 5.2.4 web application that scrapes hyperlinks from a user-provided URL. When a link is submitted through the frontend, the backend crawler processes the page, extracts all valid hyperlinks (`<a href="...">`), and displays them cleanly in the UI.

## 🚀 Features

- 🔍 Accepts a URL and crawls its content  
- 📑 Extracts and lists all anchor tag links (`<a href=...>`)  
- 🧩 Built with Django views, templates, and models  
- 📦 Clean separation of logic and UI  
- 📁 Environment variable support using `.env`

## 🛠 Tech Stack

- Python 3.11+  
- Django 5.2.4  
- `requests`, `BeautifulSoup` (for web scraping)  
- `django-environ` (for `.env` configuration)

## ⚙️ Installation

1. Clone the repository:
   git clone https://github.com/yourusername/link-collector.git
   cd link-collector

2. Create and activate a virtual environment:
   python -m venv venv
   source venv/bin/activate        # On Windows: venv\Scripts\activate

3. Install the required dependencies:
   pip install -r requirements.txt

4. Create a .env file in the project root with the following content:
   DJANGO_SECRET_KEY=your-secret-key-here

5. Apply database migrations:
   python manage.py migrate

6. Run the development server:
   python manage.py runserver

7. Open your browser and go to:
   http://localhost:8000/
