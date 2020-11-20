FROM python:3.10.0a2-alpine3.12
#RUN apt-get update && apt-get install -y python3 python3-pip
RUN pip3 install flask
WORKDIR /
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . /usr/src/app
COPY api.py /
WORKDIR /
CMD ["python3", "api.py"]
