FROM python:alpine

RUN apk --no-cache add tzdata
ENV TZ='Asia/Tokyo'

RUN pip install Flask
RUN pip install SQLAlchemy
RUN pip install flask_sqlalchemy

WORKDIR /app
COPY . /app
CMD ["python", "main.py"]

ENV LANG='ja_JP.UTF-8'
