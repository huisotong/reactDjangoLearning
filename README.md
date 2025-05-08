# reactDjangoLearning
Environment to learn React and Django.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-repo/reactDjangoLearning.git
cd reactDjangoLearning
```

### 2. Set Up the Python Environment
1. Create a virtual environment:
   ```bash
   python -m venv env
   ```
2. Activate the virtual environment:
   - On Windows:
     ```bash
     .\env\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```

3. Create a `requirements.txt` file in the root directory of the project and add the following dependencies:
   ```txt
   asgiref
   Django
   django-cors-headers
   djangorestframework
   djangorestframework-simplejwt
   PyJWT
   pytz
   sqlparse
   psycopg2-binary
   python-dotenv
   ```

4. Install the required Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### 3. Apply Migrations
1. Create migrations for the `api` app:
   ```bash
   python manage.py makemigrations
   ```
   - You should see output like:
     ```
     Migrations for 'api':
       api\migrations\0001_initial.py
         + Create model Note
     ```

2. Apply the migrations to the database:
   ```bash
   python manage.py migrate
   ```
   - You should see output like:
     ```
     Operations to perform:
       Apply all migrations: admin, api, auth, contenttypes, sessions
     Running migrations:
       Applying api.0001_initial... OK
     ```

### 4. Run the Application
- Start the Django development server:
   ```bash
   python manage.py runserver
   ```
- The server will start, and you can access the application at:
  - Backend: `http://127.0.0.1:8000/`

### 5. Deactivate the Environment
When finished, deactivate the virtual environment:
```bash
deactivate
```