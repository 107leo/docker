FROM python:3.9.7-slim

WORKDIR /app

COPY . /app

RUN pip install flask gunicorn

EXPOSE 5000

CMD ["gunicorn", "--bind", "0.0.0.0:5000", "micro1:app"]
