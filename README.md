# Inventory Management API

## Setup Instructions:
1. Clone the repository: `git clone <repo-url>`
2. Install dependencies: `pip install -r requirements.txt`
3. Setup PostgreSQL and Redis, update `settings.py`
4. Run migrations: `python manage.py migrate`
5. Start the server: `python manage.py runserver`

## API Endpoints:
- **Create Item**: `POST /items/`
- **Get Item**: `GET /items/{item_id}/`
- **Update Item**: `PUT /items/{item_id}/`
- **Delete Item**: `DELETE /items/{item_id}/`

## JWT Authentication:
- Token: `POST /token/`
- Refresh Token: `POST /token/refresh/`


**If You want to use PostgressSql or MySql as database**


DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'inventory_db',
        'USER': 'your_db_user',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}



**To run the Project use command**
python manage.py runserver 



