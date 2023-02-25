FROM python:3.10-alpine3.16
LABEL MAINTAINER="Madhu Akula" INFO="Kubernetes Goat"

COPY app.py /app.py

RUN pip install flask

EXPOSE 5000

CMD [ "python", "/app.py" ]
