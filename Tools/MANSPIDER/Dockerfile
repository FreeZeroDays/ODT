FROM ubuntu:20.04

ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update -y && apt-get upgrade -y &&  apt-get install git python3 python3-pip tesseract-ocr antiword -y
RUN git clone https://github.com/blacklanternsecurity/MANSPIDER
WORKDIR /MANSPIDER
RUN pip3 install --upgrade pip
RUN pip3 install virtualenv
RUN pip3 install -r requirements.txt
RUN sed -i 's/from .lib import */from lib import /g' /MANSPIDER/man_spider/manspider.py

ENTRYPOINT ["python3", "/MANSPIDER/man_spider/manspider.py"]
