# syntax = docker/dockerfile:1.3
FROM python:3.10
#COPY backend/requirements.txt backend/requirements.txt
COPY . /project
WORKDIR /project/backend
RUN apt-get update && apt-get install -y binutils libproj-dev gdal-bin gettext ffmpeg
RUN #--mount=type=cache,target=/root/.cache pip install -r backend/requirements.txt
RUN pip install -r requirements.txt