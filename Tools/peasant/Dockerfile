FROM python:alpine

RUN apk -U upgrade && apk add git
RUN git clone https://github.com/arch4ngel/peasant
WORKDIR /peasant
RUN pip install -r requirements.txt

ENTRYPOINT ["python", "peasant.py"]
