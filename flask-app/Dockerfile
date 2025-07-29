# Use the official Python image
FROM python:3.10-slim

# Set working directory inside the container
WORKDIR /app

# Copy requirements and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy application code
COPY app.py .

# Expose port Flask app will run on
EXPOSE 5000

# Run the Flask application
CMD ["python", "app.py"]