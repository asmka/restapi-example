FROM python:3.8.6

SHELL ["/bin/bash", "-l", "-c"]

COPY . /resource
WORKDIR /resource

RUN pip install pipenv
RUN pipenv install

CMD ["/bin/bash", "-l", "-c", "pipenv run uvicorn main:app --reload --host 0.0.0.0 --port 80"]
