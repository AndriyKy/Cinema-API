# Cinema-API
<hr>

API service for cinema management written on DRF

## Features
<hr>

- JWT authentication
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

## Installing using GitHub
<hr>

Install PostgreSQL and create DB

```bash
git clone https://github.com/AndriyKy/Cinema-API.git
cd Cinema-API
python -m venv venv
sourve venv/bin/activate
pip install -r requirements.txt
set SECRET_KEY=<your secret key>
set DJANGO_ALLOWED_HOSTS=localhost 127.0.0.1 [::1]
set SQL_ENGINE=django.db.backends.postgresql
set SQL_DATABASE=<your db name>
set SQL_USER=<your db username>
set SQL_PASSWORD=<your db password>
set SQL_HOST=<your db hostname>
set SQL_PORT=5432
python manage.py migrate
python manage.py runserver
```

### Run with Docker
<hr>

Docker should be already installed
```bash
docker-compose build
docker-compose up
```

### Getting access
<hr>

- create a user via /api/user/register/
- get access token via /api/user/token/
