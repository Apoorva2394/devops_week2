# Use an official lightweight Python image
FROM python:3.11-slim

# Set working directory in the container
WORKDIR /app

# Copy requirements then install (better for caching)
COPY requirement.txt .

RUN pip install --no-cache-dir -r requirement.txt

# Copy app code
COPY app.py .

# Expose the port the app listens on (documentation only)
EXPOSE 5000

# Command to run the app
CMD ["python", "app.py"]
