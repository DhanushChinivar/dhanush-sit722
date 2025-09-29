FROM python:3.10-slim-buster

# Set workdir
WORKDIR /code

# Copy dependencies first for caching
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy application code
COPY app /code/app

EXPOSE 8000

CMD ["python", "-m", "app.main"]
