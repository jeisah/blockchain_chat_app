FROM python:3.8.2-slim-buster
COPY ./requirements.txt /app/requirements.txt
WORKDIR /app
#RUN apt-get update -y && \
    #apt-get install -y python-pip python-dev
#RUN pip install --upgrade pip
RUN pip install -r /app/requirements.txt
EXPOSE 9090
COPY . /app
#ENTRYPOINT ["/bin/bash"] #
#RUN export FLASK_APP=node_server.py
#CMD flask run --port 9099
CMD python run_app.py
