FROM node:17-alpine

RUN npm install -g nodemon

WORKDIR /app
# Work directory of the image

COPY . .
# COPY: copy some files to the image
# The first dot(".") related path to the directory I want to copy my source file from
# Source file is the same directory as the docker file => we use "."
# If the source file is in src folder => we use "./src"
# The second dot(".") is the path inside the image I want to copy my source code to
# Path to whereever your app or index is
RUN npm install
#install all the dependancy in the package json file
EXPOSE 5000
#Tells docker whick PORT the container should expose
# required for docker desktop port mapping

CMD ["npm", "run", "dev"]
# This is the commande to run the applications "node" and "app.js" in the container