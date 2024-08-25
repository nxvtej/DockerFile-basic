# base image
FROM node:16-alpine 

# working directoy
WORKDIR /app

# then copy over files
# not optimal
COPY . .
# first . is base direcvtory this file is in 
# second . is working directory of image \app written above 

# run commands to bootstrap
RUN npm install
RUN npm run build
RUN npx prisma generate 

# port htat came up in app
EXPOSE 3000


# everything in cmd runs after 
# the image is created  (this runs when container starts)
CMD ["node", "dist/index.js"]

# command ot build image
# docker build -t demo-image . 
# . indicate root directory image file