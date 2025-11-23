FROM almalinux:9
RUN dnf install nginx -y
RUN adduser haribabu

USER haribabu
CMD ["sleep","1050"]

## We shouldn't run contianer with root access because all the containers are running on host if any user has root access he may access the underlying host storage.

## adduser command will execute with root acess after the USER instruction the next commands will execute will haribabu user.

## we are giving sleep 1050 sec to login to the container and check "id" it will show haribabu.