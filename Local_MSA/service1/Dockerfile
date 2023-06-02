FROM alpine:3.13 as tzdata
RUN apk --no-cache add tzdata
FROM python:alpine

COPY --from=tzdata /usr/share/zoneinfo /usr/share/zoneinfo

RUN pip install Flask
RUN pip install SQLAlchemy
RUN pip install flask_sqlalchemy

WORKDIR /app
COPY . /app
EXPOSE 5000
CMD ["python", "main.py"]

ENV TZ='Asia/Tokyo'
ENV LANG='ja_JP.UTF-8'