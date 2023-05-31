FROM python:alpine

RUN pip install Flask
RUN pip install SQLAlchemy
RUN pip install flask_sqlalchemy

WORKDIR /app

# ローカル環境の./app を　コンテナ環境の/appに同期
COPY ./app /app  

# コンテナのワーキングディレクトリが/appなので、/appにあるapp.pyを実行
CMD ["python", "app.py"]