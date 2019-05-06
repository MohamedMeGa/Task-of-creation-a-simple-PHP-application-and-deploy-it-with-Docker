## Mohamed MeGa




```bash
# build the docker image
docker build -t php-docker-apache-example .

# run the docker container on this machine. Expose its internal
# port 80 to this machine's port 8080
docker run -d -p 8080:80 php-docker-apache-example
```

And you can see the result here:
![screenshot](https://raw.githubusercontent.com/fuhrysteve/php-docker-apache-example/master/example.jpg)

```bash
# to spin up additional containers on different ports, you might
# do something like this:
docker run -d -p 5000:80 php-docker-apache-example
docker run -d -p 5001:80 php-docker-apache-example
docker run -d -p 5002:80 php-docker-apache-example
docker run -d -p 5003:80 php-docker-apache-example
docker run -d -p 5004:80 php-docker-apache-example
docker run -d -p 5005:80 php-docker-apache-example
docker run -d -p 5006:80 php-docker-apache-example
docker run -d -p 5007:80 php-docker-apache-example
```

