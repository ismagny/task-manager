FROM python:3.12
LABEL maintainer="Ismail Guney"
LABEL description="Image installing requirements and expose uvicorn"
LABEL version=1.0

WORKDIR /app
COPY . /app/

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
