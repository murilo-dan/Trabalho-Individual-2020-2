FROM python:3.9.4

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /api

COPY requirements.txt requirements.txt

RUN pip3 install -r requirements.txt

COPY . .