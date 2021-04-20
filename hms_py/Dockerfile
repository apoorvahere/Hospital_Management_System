FROM python:alpine3.7
RUN apk add cmd:pip3
COPY ./requirements.txt /app/requirements.txt
WORKDIR /app
RUN pip3 --cache-dir=.pip install --upgrade pip
RUN pip install -r requirements.txt
COPY . /app
ENTRYPOINT [ "python" ]
EXPOSE 5000
CMD [ "app.py" ]
