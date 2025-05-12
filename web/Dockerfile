# importing the node image 
FROM node:18  

# Creating a working directory for the app
WORKDIR /usr/src/app

# Copying the package-lock.json and package.json file to the working directory.
COPY package-lock.json /usr/src/app
COPY package.json /usr/src/app

# Installing the node dependencies
RUN npm ci 
# This will install the dependencies that are listed in the package-lock.json file

# Copying the rest of the application code to the working direectory
COPY . /usr/src/app/

CMD ["npm", "start"]
# This will start the application using the start script defined in package.json