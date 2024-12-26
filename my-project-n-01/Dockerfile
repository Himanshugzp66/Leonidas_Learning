# Use Python as the base image
FROM python:3.13

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file to the container
COPY requirements.txt .  # Ensure this file exists in the context

# Install dependencies
RUN pip install -r my-project-n-01/requirements.txt

# Copy the application code into the container
COPY . .  # Copy all files from the context to /app in the container

# Expose the port the Flask application will be listening on
EXPOSE 5000

# Run the Flask application
CMD ["python", "app.py"]
