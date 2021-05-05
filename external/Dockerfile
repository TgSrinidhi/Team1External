#FROM node:latest
#copy ./*    /home/
#WORKDIR /home

#RUN npm install
#RUN npm start
#EXPOSE 8083
#CMD [ "node", "server.js" ]

FROM node
# Create app directory
WORKDIR /app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY ./*  ./


RUN npm install


COPY . .

EXPOSE 8080

CMD [ "npm", "start" ]
