FROM node:18

WORKDIR /app
COPY ./backend-flock/package*.json ./
RUN npm install

COPY ./backend-flock .

EXPOSE 5001

CMD ["node", "server.js"]
