FROM node:alpine AS development

# Declaring env
ENV NODE_ENV development

# Setting up the work directory
WORKDIR /react-app

# Installing dependencies
COPY ./package*.json /react-app
RUN npm install

# Copying all the files in our project
COPY . .

# Exposing the port
EXPOSE 3000

# Starting our application
CMD ["npm", "start"]
