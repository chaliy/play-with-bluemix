FROM registry.eu-gb.bluemix.net/ibmnode:latest

ADD . /app
WORKDIR /app
RUN npm install

EXPOSE 3000

ENTRYPOINT ["node", "index.js"]
