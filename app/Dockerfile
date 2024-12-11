FROM python:3.7-slim

WORKDIR /app
RUN groupadd -r webservice && useradd --no-log-init -r -g webservice webservice
#RUN apt-get update && apt-get -y install curl wget busybox
COPY . .
RUN pip install -r requirements.txt

USER webservice:webservice

EXPOSE 8050
CMD ["python", "hello.py"]
