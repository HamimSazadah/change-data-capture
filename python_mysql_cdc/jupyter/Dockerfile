FROM jupyter/base-notebook

USER root 
RUN apt-get update && apt install python-dev python3-dev libmysqlclient-dev gcc -y
COPY . .

USER jovyan
RUN pip3 install --upgrade pip && pip3 install -r requirements.txt
