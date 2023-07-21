FROM node:14

WORKDIR /app/api-gateway

COPY . .

COPY package.json package-lock.json ./

RUN npm install --production

EXPOSE 3000

CMD [ "node", "app.js"]