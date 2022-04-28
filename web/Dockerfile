FROM python:3.6-slim

WORKDIR /app

COPY requirements.txt /app

RUN pip install --upgrade pip

RUN pip install -r requirements.txt

RUN pip install psycopg2-binary

COPY . .
