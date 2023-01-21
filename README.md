# Cinema-API
API service for cinema management written on DRF

## Features
- JWT authentication
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

## Installing using GitHub

```bash
git clone https://github.com/AndriyKy/Cinema-API.git
cd Cinema-API
python -m venv venv
sourve venv/bin/activate
pip install -r requirements.txt
````
- Copy **.env.sample** -> **.env** and populate with all required data

### Run locally
- Install PostgreSQL, create DB and User
- Connect DB
- Run:

```bash
python manage.py migrate
python manage.py runserver
```

### Run with Docker
Docker should be already installed
```bash
docker-compose build
docker-compose up
```

To stop:
```bash
dokcer-compose down
```

## Getting access
<hr>

- create a user via /api/user/register/
- get access token via /api/user/token/
