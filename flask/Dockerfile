#Use the Python 3.7.2 container image
FROM python:3.7.2-stretch

#Set the working dir to /app
WORKDIR /app

#Copy the current dir contents into the container at /app
ADD . /app

#Install the dependencies
RUN pip install -r requirements.txt

# run the commadn to start uWSGI
CMD ["uwsgi", "app.ini"]
