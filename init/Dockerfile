FROM debian:11-slim

RUN apt update && apt install postgresql-client curl -y

WORKDIR /app

COPY init.sh .
COPY init.sql .

RUN chmod +x init.sh

ENTRYPOINT [ "/bin/bash" ]
