FROM python:alpine

RUN pip3 install boto3
RUN mkdir -p /manage

COPY manage_jump_servers.py /manage
COPY ssh-key.pem /root/.ssh/
WORKDIR /manage

ENTRYPOINT ["python", "manage_jump_servers.py"]
