FROM nodejs:20
EXPOSE 8080
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true"\
    REDIS_URL="redis://redis:6379"
CMD [ "node", "server.js" ]