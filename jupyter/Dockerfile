FROM ubuntu:20.04

LABEL maintainer="iamvee"

COPY ./requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip install -r ./requirements.txt

ENTRYPOINT [ "jupyter-notebook" ]