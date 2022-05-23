FROM node:12

WORKDIR /app

COPY ./nodeappweb/package*.json ./

RUN npm install

COPY ./nodeappweb .

EXPOSE 8080

CMD [ "node", "server.js" ]

# git clone https://github.com/javahometech/nodeappweb.git && docker build -t 02 . && docker run -d --name node_app -p 80:8080  02