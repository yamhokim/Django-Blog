# Django Polls App

This is a basic **polls application** built using Django, following the official [Django documentation tutorials](https://docs.djangoproject.com/en/stable/intro/tutorial01/). The project demonstrates fundamental Django concepts, including models, views, templates, and testing.

## Features

- **Create Polls**: Define questions and their associated answer choices.
- **Vote**: Users can cast their votes on polls.
- **View Results**: See the results of polls in real-time.

## Requirements

- Python 3.x
- Django (version used in the tutorial: `X.X.X`)
- SQLite (default database)

## Setup and Installation

1. **Clone the repository**:

    ```bash
    git clone <repository-url>
    cd polls-app
    ```

2. **Create a virtual environment**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Run migrations to set up the database**:

   ```bash
   python manage.py migrate
   ```

5. **Run the development server**:

   ```bash
   python manage.py runserver
   ```

6. **Access the app in your web browser**:

   ```bash
   http://127.0.0.1:8000/polls/
   ```

## Recommended Project Structure

```
polls-app/
├── polls/
│   ├── migrations/
│   ├── templates/
│   │   └── polls/
│   │       ├── detail.html
│   │       ├── index.html
│   │       └── results.html
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── manage.py
└── polls-app/
    ├── settings.py
    ├── urls.py
    ├── wsgi.py
    └── asgi.py
```

## Key Features
### Models
- **Question**: Represents a poll question.
- **Choice**: Represents an answer option for a question, linked via a foreign key.

### Views
- **Index View**: Displays a list of polls.
- **Detail View**: Shows the question and choices for voting.
- **Results View**: Displays the voting results for a poll.

## Testing
Django's built-in testing framework is used to ensure the application works as expected. Run tests using:

```bash
python manage.py test
```


