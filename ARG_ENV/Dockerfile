ARG version
FROM almalinux:${version:-9} 
ARG username
RUN adduser $username
USER $username
ARG COURSE="DeVSecOps" \
    TRAINER="SIVA"
RUN echo "Course: ${COURSE}, Trainer: ${TRAINER}, Version: ${version}"
ENV COURSE=${COURSE}
ENV TRAINER=${TRAINER}
CMD ["sleep","1000"]


## ARG instruction will pass the arguments while building the image. We are not hard coding and pass the values in command.
## ENV can pass the arguments while building image and running container.

##To pass the VERSION,username,course,trainer during building an image
## docker build -t arg:v1 --build-arg version=9 --build-arg username=haribabu --build-arg COURSE=DevSecOps --build-arg TRAINER=SIVA .


##Run command will take the username from ARG and to ARG instruction we are passing via commnad during build.

## How can I use ARG variables inside container?
## Assign the values of ARG to ENV variables so that you can access them inside container as well

## Other than FROM we can user ARG as first instruction.
## ARG instruction can be used before FROM instruction to provide values to FROM instruction.

## ARG value defined before FROM will not be accessed after FROM