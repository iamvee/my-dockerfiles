FROM ubuntu:20.04

LABEL maintainer="iamvee"

RUN apt-get update && \
    apt-get install python3.8 python3-pip -y 

COPY ./requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip3 install -r ./requirements.txt

EXPOSE 8080

# ENTRYPOINT [ "jupyter" ]
# VOLUME ./data:/root/data
WORKDIR /root
USER root
ADD ./data /root/data

CMD jupyter notebook --ip 0.0.0.0 --port 8080  --allow-root

