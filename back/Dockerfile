FROM python:3.8.1
ENV PYTHONUNBUFFERED 1
WORKDIR /app
COPY ./demoapp/Pipfile /app/Pipfile
COPY ./demoapp/Pipfile.lock /app/Pipfile.lock
RUN pip install pipenv
RUN pipenv install
EXPOSE 8000
ENTRYPOINT pipenv run python manage.py runserver 0.0.0.0:8000
