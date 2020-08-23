FROM ubuntu:latest

RUN apt-get update && apt-get install python3 -y \
    && apt-get -y install python3-pip 

WORKDIR /app

COPY . /app

RUN pip3 --no-cache-dir install -r requirements.txt 

EXPOSE 5000

CMD ["python3","app.py"]

