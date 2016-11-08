FROM node:argon
EXPOSE 80

WORKDIR /app
COPY package.json .
RUN npm install
COPY . .

RUN useradd -ms /bin/bash peterj

CMD ["node", "server.js"]
