FROM python:3.9.7-slim

WORKDIR /app

COPY . /app

RUN pip install flask gunicorn

EXPOSE 5000

CMD ["gunicorn", "-w", "4", "-b", "0.0.0.0:5000", "--timeout", "120", "micro1:app"]
