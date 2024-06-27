FROM python:3.11-slim
WORKDIR /app
COPY . /app
RUN apt-get update && apt-get install -y python3-opencv
RUN pip install opencv-python
RUN pip install -r requirements.txt
ENV REDACTOR_HOST REDACTOR_PORT
EXPOSE 5556
CMD ["python" , "-m" ,"app"]
