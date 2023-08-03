FROM node:16

WORKDIR /app

COPY package.json package*.json ./

RUN npm install

COPY . .

# COPY ../lib-p3 /app/lib-p3

CMD [ "npm", "start" ]
