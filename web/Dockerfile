#docker image of web
# VERSION 1.0
# Author: donghaixing

FROM python:3.6
ENV PYTHONUNBUFFERED 1
WORKDIR /code/ihasy
ADD ./codes/ihasy /code/ihasy
RUN pip install -r requirements.txt -i http://pypi.douban.com/simple/ --trusted-host pypi.douban.com
CMD ["python", "/code/ihasy/application.py"]