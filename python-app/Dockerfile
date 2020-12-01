FROM ubuntu:18.04

WORKDIR /code

COPY requirements.txt .
RUN apt-get update && apt-get install -y \
    vim \
    python3 \
    python3-pip
RUN pip3 install -r requirements.txt

COPY . .

CMD [ "python3", "./app/server.py" ]
#EXPOSE 5000/tcp