# Use the official Node.js image as the base image
FROM node:18 as build

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install project dependencies
RUN npm install
RUN npm install -g @angular/cli
# Copy the entire project to the container
COPY . .
#La commande ng build --configuration production place les fichiers générés dans le dossier dist/<nom-du-projet>
# Build the Angular app for production
RUN ng build --configuration production


# Use a smaller, production-ready image as the final image
FROM nginx:alpine

# Copy the production-ready Angular app to the Nginx webserver's root directory

COPY --from=build /app/dist/besmelh-ra7men-ra7im/browser /usr/share/nginx/html
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]