FROM python:alpine

RUN pip install Flask
RUN pip install SQLAlchemy
RUN pip install flask_sqlalchemy

WORKDIR /app

COPY . /app

EXPOSE 5000

CMD ["python", "main.py"]
