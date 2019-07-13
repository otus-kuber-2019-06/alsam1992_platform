FROM python:3.7

RUN mkdir /app

COPY app/homework.html /app

WORKDIR /app

EXPOSE 8000

USER 1001

CMD ["python3", "-m", "http.server", "8000"]