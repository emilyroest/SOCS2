FROM node:18

WORKDIR /app

# Copy root-level package files (backend package.json is in root)
COPY package*.json ./

RUN npm install

# Copy only backend code
COPY ./backend-flock ./backend-flock

WORKDIR /app/backend-flock

EXPOSE 5001

CMD ["node", "server.js"]
