FROM python:latest


WORKDIR /app

COPY . .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

ENTRYPOINT gunicorn --bind 0.0.0.0:5000 app:app