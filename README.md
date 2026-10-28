# Flask Blog Website

A responsive blog website developed using Python, Flask, Jinja2, and Bootstrap. The application displays dynamic blog content and provides a contact form for visitors.

## Features

- Dynamic blog posts rendered with Jinja2 templates
- Individual pages for blog posts
- Responsive interface using Bootstrap
- Contact form with POST request handling
- Email notifications through SMTP (when configured)
- Reusable HTML templates

## Technologies

- **Backend:** Python, Flask
- **Frontend:** HTML, CSS, Bootstrap
- **Templating:** Jinja2
- **HTTP Requests:** Requests
- **Email:** Python SMTP library

## Project Structure

```text
flask-blog/
├── static/
│   └── assets/
├── templates/
│   ├── index.html
│   ├── post.html
│   ├── about.html
│   ├── contact.html
│   ├── header.html
│   └── footer.html
├── main.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

## Installation

**1. Clone the repository**

```bash
git clone https://github.com/mhmd-mehrdad/flask-blog.git
cd flask-blog
```

**2. Create a virtual environment**

```bash
python -m venv .venv
```

**3. Activate the environment**

Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

**4. Install dependencies**

```bash
pip install -r requirements.txt
```

**5. Configure environment variables**

Copy `.env.example` to `.env` and configure the required credentials if email notifications are enabled.

**6. Run the application**

```bash
python -m flask --app main run --debug
```

Open `http://127.0.0.1:5000` in your browser.

## Contact Form

Visitors can submit messages using the contact form. Flask processes the submitted information through an HTTP POST request.

When SMTP is configured, the application can send submitted messages to the configured email address.

## Future Improvements

- Database integration for storing blog posts
- User authentication
- Admin dashboard for managing posts
- Pagination and search functionality

## Author

**Mehrdad Mohammadi**

GitHub: [mhmd-mehrdad](https://github.com/mhmd-mehrdad)