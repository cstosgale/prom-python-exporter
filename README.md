# Docker container for running a Python Script

This project provides you with a docker container which can be used to run python code. It includes building it with any required libraries installed via pip.

This project is built with:

- The latest python version
- Any additional packages you require, please modify the requirements.txt file to adjust what is included

And is packaged as a Docker container.

## Building

To build manually:

`docker build -t python-docker .`

## Running

Simply open port 8000 when running as a container:

`docker run -p 8000:8000 --name python-docker cstosgale/python-docker`

When the app runs, it will attempt to run /app.py, this is your python file. Be sure to redirect this to your file outside the container in order for it to run your code.
