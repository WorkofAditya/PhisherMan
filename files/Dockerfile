# Use official Python 3 base image (Debian-based)
FROM python:3

# Set working directory inside the container
WORKDIR /PhisherMan

# Copy all local files into the container
ADD . /PhisherMan

# Install system dependencies
RUN apt-get update && \
	apt-get install -y php openssh-client && \
	apt-get clean

# Install Python dependencies
RUN pip install --no-cache-dir -r files/requirements.txt

# Run the script when the container starts
CMD ["python3", "phisherman.py", "--noupdate"]
