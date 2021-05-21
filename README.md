# FastAPI with elasticsearch on docker container

This repo contains demo code that tell you how we can use fastapi with docker and connected with elasticsearch(As a database).

**Tech stack:**

1.FastAPI

2.Elasticsearch

3.docker

**Steps to run**

1. Pull code or download the code(It is public repo)
2. If you have docker on your system then just run single command

    **docker-compose up --build**

Note- Be ensure you are in directory where Dockerfile and yml is there.

**Api endpoints for trade**

1. Get trade based on trade id

    **URL- http://{IP}:8001/trade/{trade_id}**

    Method- GET

    eg: trade_id = 332

2. Get list of trades

    **URL- http://{IP}:8001/trade/?page=1**

    Method- GET

3. Search on many fields (As mentioned in Assgnment)

    **URL- http://{IP}:8001/trade/?keyword=Banglore&page=1**

    **Method- GET**

3. Filter

    **http://{IP}:8001/trade/?page=1&start=2015-02-11 00:00:00&end=2016-02-11 01:12:00**


**Note- Please change IP(In app/es_connector.py) assigned to elastisearch container in your machine.**
