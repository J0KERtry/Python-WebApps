FROM python:alpine

RUN pip install Flask \
    && pip install SQLAlchemy \
    && pip install flask_sqlalchemy

WORKDIR /app
COPY . /app
CMD ["python", "main.py"]

ENV LANG='ja_JP.UTF-8'