FROM node:argon

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Bundle app source
#COPY . /usr/src/app
RUN git clone https://github.com/danvy/hackitdocker
WORKDIR /usr/src/app/hackitdocker

# Install app dependencies
# COPY package.json /usr/src/app/
RUN npm install

EXPOSE 80
CMD [ "npm", "start" ]
