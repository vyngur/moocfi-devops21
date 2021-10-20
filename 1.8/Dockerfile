# Start with Ubuntu 18.04
FROM ubuntu:18.04

# Update apt cache
RUN apt update && apt upgrade -y

# Install curl
RUN apt install curl -y

# Use /usr/src/app as our workdir, The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the curler script
COPY curler.sh .

# Set as executable
RUN chmod +x ./curler.sh

# Run it
CMD ./curler.sh