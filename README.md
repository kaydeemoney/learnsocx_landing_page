# LearnSocx: Social Media Marketing Training Platform



## Overview

**LearnSocx** is an advanced social media marketing platform designed to empower users with skills across multiple platforms, including **Facebook**, **Instagram**, **Twitter**, and **YouTube**. The platform offers comprehensive marketing courses, practical assignments, and real-time analytics to track progress.

## Features

- 📈 **Real-time Analytics**: Track your learning progress and engagement with interactive visualizations.
- 🎥 **Video Tutorials**: Step-by-step video guides to navigate each social platform.
- 📚 **Comprehensive Content**: Includes in-depth modules for Facebook Ads, Instagram Stories, Twitter Growth Hacks, and more.
- 🚀 **Practical Assignments**: Real-world marketing tasks to enhance learning through hands-on experience.
- 🔒 **Secure Platform**: Robust security protocols including password encryption and data privacy.

## Technology Stack

| Frontend      | Backend         | Database        | DevOps          |
|---------------|-----------------|-----------------|-----------------|
| HTML5, CSS3   | Python (Flask)   | MySQL           | Nginx           |
| JavaScript    | SQLAlchemy       | AWS RDS         | Gunicorn        |
| Bootstrap     | Jinja Templates  | SQLAlchemy ORM  | Docker          |

## Installation

### Prerequisites

Ensure you have the following installed:

- **Python 3.8+**
- **MySQL**
- **Git**
- **Virtualenv**

### Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/learnsocx.git
    cd learnsocx
    ```

2. Set up a virtual environment:
    ```bash
    virtualenv venv
    source venv/bin/activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Configure the database in `config.py`:
    ```python
    SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://<username>:<password>@localhost/<database_name>'
    ```

5. Initialize the database:
    ```bash
    flask db init
    flask db migrate
    flask db upgrade
    ```

6. Run the application:
    ```bash
    flask run
    ```

## Usage

- Visit the **landing page** at `http://localhost:5000/` to access the main platform.
- **Admin panel**: `/admin` (requires login).
- **Student dashboard**: `/dashboard`.

## Project Structure

```bash
├── app/
│   ├── static/         # CSS, JS, Images
│   ├── templates/      # HTML templates
│   ├── models.py       # Database models
│   ├── routes.py       # Flask routes
│   ├── forms.py        # Flask-WTF forms
│   └── __init__.py     # App initialization
├── migrations/         # Database migrations
├── tests/              # Unit tests
├── config.py           # Configuration file
├── requirements.txt    # Python dependencies
