FROM node:8.15

WORKDIR /opt/friends
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run prestart
EXPOSE 8080
ENV DEBUG=cloudstate*
ENTRYPOINT [ "npm", "run", "start-no-prestart" ]
