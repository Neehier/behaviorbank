FROM python:3.8

COPY . /app

RUN apt update

RUN apt install ffmpeg -y
RUN pip install youtube_dl azure-storage-blob azure-cosmos PyYAML pytz

WORKDIR /app

CMD ["python", "bb-frames-extractor.py"]