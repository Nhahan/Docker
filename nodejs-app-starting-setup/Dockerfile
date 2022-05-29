FROM node

WORKDIR /app

# Copy package.json to the container for saving build time
COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

CMD ["node", "server.js"]

# docker run -p ${localport}:${dockerport} ${hash}
# docker run -p 3000:80 ${hash}
# By default, if you run a Container without -d, you run in "attached mode