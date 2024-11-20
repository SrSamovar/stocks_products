FROM python:3.12-slim

COPY requirements.txt .

RUN pip3 install -r requirements.txt

COPY . .

ENV MY_ENV=docker
EXPOSE 8000

CMD ["sh", "-c", "python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]