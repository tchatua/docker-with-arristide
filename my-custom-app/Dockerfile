# my-custom-app

FROM ubuntu

RUN apt-get update
RUN apt-get -y install python2-minimal python2 dh-python 2to3 python-is-python3
RUN apt-get -y install python-pip
RUN apt-get -y  install pip
RUN pip install flask

COPY app.py /opt/app.py

ENTRYPOINT FLASK_APP=app.py flask run --host=0.0.0.0