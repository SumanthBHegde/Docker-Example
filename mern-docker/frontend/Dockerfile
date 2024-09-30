# set the base image to create the image for react app
FROM node:20-alpine

# RUN addgroup app && adduser -S -G app app

# set the user to run the app
# USER app

# set the working directory to /app
WORKDIR /app

COPY package*.json ./

# USER root

# RUN chown -R app:app .

# change the user back to the app user
# USER app

# install dependencies
RUN npm install

# copy the rest of the files to the working directory
COPY . .

# expose port 5173 to tell Docker that the container listens on the specified network ports at runtime
EXPOSE 5173

# command to run the app
CMD npm run dev