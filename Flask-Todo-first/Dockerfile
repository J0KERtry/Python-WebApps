FROM python:alpine

RUN pip install Flask
RUN pip install SQLAlchemy
RUN pip install flask_sqlalchemy

WORKDIR /app

COPY ./app /app

CMD ["python", "app.py"]