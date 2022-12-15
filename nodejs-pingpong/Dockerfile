FROM node
COPY app/Ping-Pong.js /opt
WORKDIR /opt
RUN npm install express cors
CMD ["node", "Ping-Pong.js"]
EXPOSE 3001
