# Pull base image
FROM python:3.10

# SET environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFED 1

# Set work directory
WORKDIR /code

# Install dependencies
COPY Pipfile Pipfile.lock /code/
RUN pip install pipenv && pipenv install --system

# Copy project
COPY . /code/