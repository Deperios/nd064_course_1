# Use Python 3.8 base image
FROM python:3.8

# Set working directory
WORKDIR /app

# Copy project files
COPY . /app

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Initialize the database
RUN python init_db.py

# Expose port 3111
EXPOSE 3111

# Start the application
CMD ["python", "app.py"]