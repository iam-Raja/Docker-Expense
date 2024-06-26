FROM node:20
EXPOSE 8080
ENV DB_HOST=mysql
RUN adduser expense
RUN mkdir /opt/server
RUN chown expense:expense -R /opt/server
WORKDIR /opt/server
COPY package.json .
RUN npm install
COPY *.js .
CMD [ "node","index.js"]
 

