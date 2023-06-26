FROM node:18-alpine
#? Working directory (in the container)
WORKDIR /app
#? Copy package*.json and package-lock,json for configuration
COPY package*.json ./
#? Install project dependencies
RUN npm install 
#? Copy entire project to the container directory
COPY . .
#? Expose the port where the NestJS application is running
EXPOSE 3000
#? Variable MongoDB variables for connection
ENV MONGO_HOST mongodb+srv://admin:tolucajs123admin@blognews.95rqp73.mongodb.net/
#? ENV MONGO_DB blognews
#? Start NestJS application
CMD ["npm", "run", "start"]

