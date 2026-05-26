FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y python3 python3-pip

RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

WORKDIR /app

COPY ./app /app/

CMD ["python3", "/app/api.py"]