FROM python:3.11-slim

WORKDIR /app

COPY ../../shared/requirements.txt .
RUN pip install __no_cache_dir -r requirements.txt

COPY src ./src

WORKDIR /app/src

ENTRYPOINT ["python", "manage.py", "runserver", "0.0.0.0:8000"]

