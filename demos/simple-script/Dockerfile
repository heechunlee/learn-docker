# Defines base Image
# Tag after Image name specifies version
FROM alpine:3.13

# Specifies /usr/src/app as working directory within Container of Docker Host 
WORKDIR /usr/src/app 

# Copies weiyi.sh script from local path into WORKDIR directory
COPY weiyi.sh .

# Gives permission to run weiyi.sh script
RUN chmod +x weiyi.sh

# Runs weiyi.sh from WORKDIR
CMD ./weiyi.sh

