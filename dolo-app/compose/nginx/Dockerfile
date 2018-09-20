#######################################################
# Dockerfile to build a nginx image
# Build by command: "docker build -t my-nginx ."
# Run by command: "docker run --name my-nginx-instance -P -d my-nginx"
#######################################################
# Base image is nginx
FROM nginx

# Author: Mr. Loi Trinh
MAINTAINER Mr. Loi Trinh <loi.trinhxuan@asnet.com>

# Data volume
VOLUME /var/log/nginx

# Expose port 80, 443
EXPOSE 80 443

# Launch nginx server in the foreground
CMD ["nginx", "-g", "daemon off;"]
