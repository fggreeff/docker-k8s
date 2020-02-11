FROM node:alpine

# This will be the new working directory, if it doesn't exist, it will be created
WORKDIR /usr/app 

# Only copy package.json so we can make changes to our code and the package can be fetched from cache
COPY ./package.json ./
# RUN npm install 
RUN npm install

# This will happen in the workdir specified above
COPY ./ ./

CMD  ["npm", "start"]