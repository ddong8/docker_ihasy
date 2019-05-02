#docker image of web
# VERSION 1.0
# Author: donghaixing

FROM python:3.6

ENV PYTHONUNBUFFERED 1

RUN mkdir /var/log/ork
RUN chmod -R 777 /var/log/ork
RUN mkdir /etc/ork

WORKDIR /code/ork

COPY /code/ork/etc/ork.json /etc/ork/ork.json

RUN pip install -r requirements.txt -i https://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com
CMD ["python", "/code/ork/start_up.py"]