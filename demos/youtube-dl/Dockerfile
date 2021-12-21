# Defines base Image
# Tag after Image name specifies version
FROM ubuntu:18.04 

# Specifies /usr/src/app as working directory within Container of Docker Host 
WORKDIR /usr/src/app

# Installs dependencies 
RUN apt-get update 
RUN apt-get install -y curl python 

# Installs youtube-dl to path /usr/local/bin in Container and gives permission to run build 
RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
RUN chmod a+x /usr/local/bin/youtube-dl

# Sets environment variable for localization settings
ENV LC_ALL=c.UTF-8 

# Runs /usr/local/bin/youtube-dl that accepts URL as single argument 
ENTRYPOINT ["/usr/local/bin/youtube-dl"]

