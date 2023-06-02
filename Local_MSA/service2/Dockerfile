FROM python:alpine

RUN apk --no-cache add build-base libffi-dev openssl-dev
RUN pip install --no-cache-dir -r requirements.txt
RUN apk del build-base libffi-dev openssl-dev

WORKDIR /app

COPY . /app

EXPOSE 5000

CMD ["python", "main.py"]
