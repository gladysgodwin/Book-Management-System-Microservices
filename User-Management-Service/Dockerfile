FROM node:14

WORKDIR /app/user-management

COPY . .

COPY package.json package-lock.json ./

RUN npm install --production

COPY MongoDB-Config.txt .

EXPOSE 4000

CMD [ "node", "app.js"]