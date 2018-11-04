# use official python dev image provided by docker 
FROM python:2.7-slim

# switch work directory
WORKDIR /app

# copy all files in current path to /app
ADD . /app

# install dependency with pip
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# allow to access docker container from port 80 from external env
EXPOSE 80

# set env variable
ENV NAME World

# set progress in container to python app.py
CMD ["python", "app.py"]
