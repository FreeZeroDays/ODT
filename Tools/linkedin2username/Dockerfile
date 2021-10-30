FROM python:alpine

RUN apk -U upgrade && apk add git
RUN git clone https://github.com/initstring/linkedin2username
WORKDIR /linkedin2username
RUN pip install -r requirements.txt

ENTRYPOINT ["python", "linkedin2username.py"]
