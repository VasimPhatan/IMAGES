FROM node:20 
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"
    
CMD ["node", "server.js"]