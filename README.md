# Dockerizing Cinema API

API service for cinema management written on DRF

## Installing using Github

```shell
git clone https://github.com/MarkoKhodan/dokerized-cinema-api.git
cd dokerized-cinema-api
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB_HOST=db
set DB_NAME=app
set DB_USER=postgres
set DB_PASSWORD=password
set SECRET_KEY=django-insecure-6vubhk2$++agnctay_4pxy_8cq)mosmn(*-#2b^v4cgsh-^!i3
python manage.py runmigtarions
python manage.py runserver
```
### Run with docker

```shell
docker-compose build
docker-compose up
```

Getting access
-
- create user via /api/user/register/
- get access token via /api/user/token/


Features
-
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors and image
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions