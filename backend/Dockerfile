FROM python:3.13.7-slim

# Create working directory
WORKDIR /app

# System deps for PostgreSQL driver (if needed)
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    gcc \
    libpq-dev \
 && rm -rf /var/lib/apt/lists/*

# Copy only requirements first (cache)
COPY requirements.txt ./
RUN pip install --upgrade pip && pip install -r requirements.txt

# Copy app (to be added in next step)
COPY . /app

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]