FROM python:3.8-slim

WORKDIR /app

COPY . .

RUN apt-get update \
    && apt-get install gcc -y \
    && apt-get clean

RUN pip install -r requirements.txt \
    && rm -rf /root/.cache/pip

COPY . /app/
