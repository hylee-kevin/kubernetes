# Use the Ubuntu base image
FROM Ubuntu

# Update apt repository
RUN apt-get update

# Install dependencies using apt
RUN apt-get install -y python

# Install Python dependencies using pip
RUN pip install flask
RUN pip install flask-mysql

# Copy source code to /opt folder
COPY . /opt/source-code

# Set the working directory
WORKDIR /opt/source-code

# Specify entry point to run the web server
ENTRYPOINT ["flask", "run"]
