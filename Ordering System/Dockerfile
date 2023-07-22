FROM python:3.9-slim

WORKDIR /app/ordering-system

COPY requirements.txt requirements.txt

RUN pip3 install -r requirements.txt

RUN pip3 install psycopg2-binary pika requests mysql-connector

COPY . .

EXPOSE 8080

CMD [ "python3", "order.py", "stock.py"]