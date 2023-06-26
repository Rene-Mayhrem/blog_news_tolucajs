FROM node:18-alpine
#? Working directory (in the container)
WORKDIR /app
#? Copy package*.json and package-lock.json for configuration
COPY package*.json ./
#? Install project dependencies
RUN npm install
RUN npm install -g http-server
#? Copy entire project to the container directory
COPY . .
#? Build VueJS application
RUN npm run build
#? Used port for vuejs application
EXPOSE 8080
#? Start nginx server
CMD ["http-server", "dist"]
