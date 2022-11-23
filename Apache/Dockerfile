From ubuntu 
MAINTAINER qhagayla <qhagayla@tip.edu.ph>

# Skips prompts
ARG DEBIAN_FRONTEND=noninteractive

# Update packages
RUN apt update; apt dist-upgrade -y

# Install packages
RUN apt install -y apache2 libapache2-mod-php 

# Clean
RUN apt clean

# Port  
EXPOSE 80

# Set CMD 
CMD ["apache2ctl", "-D", "FOREGROUND"]
