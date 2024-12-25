# Base image
FROM python:3.13

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file to the working directory
COPY requirements.txt .  # Copies requirements.txt from the context to /app

# Install the project dependencies
RUN pip install -r requirements.txt

# Copy the entire application code into the container
COPY . .  # Copies all files in the current folder to /app

# Expose the port the Flask application will be listening on
EXPOSE 5000

# Run the Flask application
CMD ["python", "app.py"]
