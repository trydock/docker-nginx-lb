# nginx-lb

a stupid nginx load balancer to be used with docker

  - There is only one public IP
  - Try multiple docker containers
  - Get config from a git repo

Todo:
  - improvements and clean up

## warning

> Not Production Ready, STUPID PIECE OF CODE

### Version
0.0.1.shit-release

### Tech

nginx-lb uses a number of open source projects to work properly:

* [nginx] - nginx [engine x] is an HTTP and reverse proxy server.
* [supervisord] - Supervisord allows users to monitor and control UNIX processes .

### Docker
docker-nginx-lb is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 80, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
docker run --name nlb01 -d -p 80:80 --restart="always" trystack/docker-nginx-lb:latest
```

This will launch the 'docker-nginx-lb'.
Verify the 'docker-nginx-lb' is online by navigating to your server address in your preferred browser.


### License

GNU/GPL3

#### Contact

Debuggerboy 
a.k.a Anish.Asokan
asokan(dot)anish(at)gmail(dot)com
