FROM python:3.11-slim
WORKDIR /app
COPY . /app
RUN apt-get update && apt-get install -y python3-opencv
RUN pip install opencv-python
RUN pip3 install -r requirements.txt
ENV PLAYBACK_HOST=18.171.177.228 PLAYBACK_PORT=5555 REDACTOR_PORT=5556 
EXPOSE 5556
CMD ["python" , "-m" ,"app"]
