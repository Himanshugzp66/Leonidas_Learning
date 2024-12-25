# Base image
FROM python:3.13

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file to the working directory
COPY requirements.txt .  # Ensure requirements.txt is in the same directory as the Dockerfile

# Install the project dependencies
RUN pip install -r my-project-n-01/requirements.txt  # Corrected the path here

# Copy the entire application code into the container
COPY . .  # Copy the entire application

# Expose the port the Flask application will be listening on
EXPOSE 5000

# Run the Flask application
CMD ["python", "app.py"]
