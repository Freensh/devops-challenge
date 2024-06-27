FROM python:3.11-slim
WORKDIR /app
COPY . /app
RUN apt-get update && apt-get install -y python3-opencv
RUN pip install opencv-python
RUN pip3 install -r requirements.txt
EXPOSE 5555
CMD ["python" , "-m" ,"app"]
