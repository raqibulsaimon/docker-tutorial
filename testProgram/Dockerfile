#use an official python image
FROM python:2.7-slim

#set the working directory to /app
WORKDIR /app

#copy the current directory contents into the containers at /app
ADD . /app

#install any needed packages specified in the requirements.txt file
RUN pip install --trusted-host pypi.python.org -r requirements.txt

#Make port 80 available to the world outside of containers
EXPOSE 80

#define environment variable
ENV NAME world

# Run app.py when container lunch

CMD ["python","app.py"]
