FROM python:3.13-alpine

RUN apk add --no-cache libxml2-dev libxslt-dev \
    && apk add --no-cache --virtual .build_deps build-base libffi-dev \
    && pip install --no-cache-dir --upgrade pip \
    && pip install --no-cache-dir --upgrade parsedmarc \
    && apk del .build_deps
