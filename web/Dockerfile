FROM python:3.7.6-stretch

WORKDIR /

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY . /

RUN pip install --upgrade pip
RUN pip install -r requirements.txt && pip install gunicorn

ENTRYPOINT ["/runserver.sh"]