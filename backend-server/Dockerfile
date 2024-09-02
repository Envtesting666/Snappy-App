# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file into the container
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the current directory contents into the container at /app
COPY . .

# Set environment variables
ENV MONGO_URL="mongodb+srv://fatihakkaya:JL3LmTHwtbOKo1yw@cluster0.l2he0.mongodb.net/myDatabase?retryWrites=true&w=majority&appName=Cluster0"

# Expose the port that the Flask app runs on
EXPOSE 5000

# Command to run the Flask app
CMD ["python", "index.py"]
