# Base image
FROM python:3.13

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file to the working directory (adjust the path if needed)
COPY my-project-n-01/requirements.txt .  # If the requirements.txt is inside a subfolder

# Install the project dependencies
RUN pip install -r requirements.txt  # Use the relative path to requirements.txt

# Copy the entire application code into the container
COPY . .  # Copy the entire application

# Expose the port the Flask application will be listening on
EXPOSE 5000

# Run the Flask application
CMD ["python", "app.py"]
