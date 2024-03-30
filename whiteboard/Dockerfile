FROM ubuntu:20.04

# Copy the entire server folder into the container
COPY . .

RUN	apt-get update && apt-get install -y curl 
RUN	curl -fsSL https://deb.nodesource.com/setup_14.x | bash -
RUN	apt-get install -y nodejs


RUN cd /client && npm install -g socket.io && npm install 
RUN cd /backend && npm install
