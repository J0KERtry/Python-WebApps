FROM python:alpine

RUN pip install --upgrade pip
RUN pip install Flask
RUN pip install SQLAlchemy

WORKDIR /app

COPY ./app /app

CMD ["python", "app/app.py"]