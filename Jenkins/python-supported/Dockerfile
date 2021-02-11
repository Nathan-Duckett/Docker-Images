# Pull in python binaries
FROM python:3.8 as python_layer

# Pull Jenkins after building on python to load jenkins after
FROM jenkins/jenkins:latest

USER root

# Copy python from initial python_layer to jenkins
COPY --from=python_layer /usr/bin/python3.8 /usr/bin/python3