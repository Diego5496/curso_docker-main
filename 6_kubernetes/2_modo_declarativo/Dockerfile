FROM python:3

RUN apt-get update && apt-get install -y \
    software-properties-common
RUN apt-get update && apt-get install -y \
    apache2 \
    curl \
    git \
    python3.4 \
    python3-pip
WORKDIR /app

RUN pip install Flask

COPY . .

EXPOSE 5000

CMD [ "python", "./app.py"]