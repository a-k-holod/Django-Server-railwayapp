## Django Template

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/GB6Eki?referralCode=U5zXSw)


python3 -m venv myenv

source myenv/bin/activate

pip freeze > requirements.txt


python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver 

docker-compose run django python manage.py makemigrations
docker-compose run django python manage.py migrate


docker-compose build
docker-compose up


curl --location 'http://localhost:8000/api/categories/' \
--header 'Content-Type: application/json' \
--data '{"name": "Electronics"}'