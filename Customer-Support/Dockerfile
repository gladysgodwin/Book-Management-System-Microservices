FROM python:3.9-slim

WORKDIR /app/customer-support

COPY . .

RUN apt-get update && apt-get install -y nodejs npm

RUN npm install

EXPOSE 8088

CMD [ "python", "server.py" ]