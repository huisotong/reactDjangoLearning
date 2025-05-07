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

### 3. Run the Application
- Start the Django development server:
   ```bash
   python manage.py runserver
   ```

### 4. Deactivate the Environment
When finished, deactivate the virtual environment:
```bash
deactivate
```