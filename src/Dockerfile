# # Use the official Node.js 14 image as the base image
# FROM node:14 AS build

# # Set the working directory in the container
# WORKDIR /app

# # Copy package.json and package-lock.json (or yarn.lock) into the container
# COPY ./package*.json ./

# # Install dependencies
# RUN npm install --force --prefer-offline --no-audit

# # Copy the rest of the application code into the container
# COPY ./ .

# # Build the Angular application
# RUN npm run build

# # Use a lightweight web server to serve the application
# FROM nginx:alpine

# # Copy the built Angular application from the previous stage
# COPY --from=build /app/dist/ /usr/share/nginx/html

# # Expose port 80 for the web server
# EXPOSE 80

# # Start Nginx
# CMD ["nginx", "-g", "daemon off;"]

FROM nginx:alpine
COPY index.html /usr/hsare/nginx/html
