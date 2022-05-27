FROM node

WORKDIR /app

COPY . /app

RUN npm install

EXPOSE 80

CMD ["node", "server.js"]

# docker run -p ${localport}:${dockerport} ${hash}
# docker run -p 3000:80 ${hash}