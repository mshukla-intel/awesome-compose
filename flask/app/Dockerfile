FROM openvino/ubuntu18_dev
USER root
RUN apt-get update && apt-get install -y git python3-pip
#FROM python:3.8-ubi8
WORKDIR /app 
COPY requirements.txt /app
RUN pip3 install -r requirements.txt --no-cache-dir
COPY . /app 
ENTRYPOINT ["python3"] 
CMD ["app.py"]
