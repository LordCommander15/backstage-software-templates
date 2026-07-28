FROM python:3.12-alpine

COPY ./requirements.txt /tmp

RUN pip install -r /tmp/requirements.txt

COPY source /source

CMD python /source/app.py