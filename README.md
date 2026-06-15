# CyberShield – GUI Based Cybersecurity Toolkit

CyberShield is a multi-page web application built using the Django framework, developed as part of the AICT semester project. The project focuses on graphical user interface (GUI) design and framework-based web development, using a modern, animated, cyber-themed interface to present a collection of practical cybersecurity tools.

## Project Focus

This project emphasizes:

- **Framework-driven development** using Django's Model-View-Template (MVT) architecture, with separate apps for core navigation (`main`) and tool functionality (`tools`)
- **Multi-page navigation** with dedicated pages for login, registration, dashboard, and individual tools
- **Modern, animated GUI design** built with Bootstrap, custom styling, scroll animations, and a particle background effect
- **Clean separation** between page structure (HTML templates), styling (CSS), and backend logic (Django views)

## Tech Stack

**Backend**
- Django (Python web framework)
- SQLite database

**Frontend**
- Bootstrap 5 & Bootstrap Icons
- Custom CSS (`style.css`)
- Google Fonts: Orbitron, Share Tech Mono, Poppins
- AOS (Animate On Scroll) for entrance animations
- Particles.js for animated background effects

**Additional Libraries**
- `dnspython` – DNS lookups
- `python-whois` – WHOIS domain lookups
- `psutil` – system and process information
- `requests` – HTTP requests for external data

## Project Structure

```
cybershield/
├── config/              # Django project configuration
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── main/                 # Core app - authentication, dashboard, navigation
├── tools/                # Cybersecurity tool modules and API endpoints
├── templates/
│   └── base.html         # Shared base layout for all pages
├── static/
│   └── css/style.css     # Custom styling
├── manage.py
├── requirements.txt
└── db.sqlite3
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ahsan-it/CyberShield-AICT-Project.git
cd CyberShield-AICT-Project/cybershield
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Apply database migrations

```bash
python manage.py migrate
```

### 4. Run the development server

```bash
python manage.py runserver
```

The application will be available at `http://127.0.0.1:8000/`.

## Application Routes

| URL | Description |
|-----|-------------|
| `/` | Main app routes (login, dashboard, tool pages) |
| `/admin/` | Django admin panel |
| `/api/` | Tools API endpoints |

## Team

This project was developed as a group submission for the AICT course.

- Ahsan – Password and Encryption Tools, GUI Pages
- Zunaira
- Unaiza
- Hussain

## License

This project was created for academic purposes as part of a university course assignment.
