FROM debian
# Copy application files
COPY . /app
# Install required system packages
RUN apt-get update
RUN apt-get -y install imagemagick curl software-properties-common gnupg vim ssh
RUN curl -sL https://deb.nodesource.com/setup_20.x | bash -
RUN apt-get update
RUN apt-get install -y nodejs
# Install NPM dependencies
RUN npm install --prefix /app
EXPOSE 80
CMD ["npm", "start", "--prefix", "app"]
