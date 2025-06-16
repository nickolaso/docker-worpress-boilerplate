# docker-worpress-boilerplate
Simple Docker Wordpress Example for starting new projects.  Includes HTTPS

- Adding a domain name or using "http://localhost:8080"
- Having a valid "HTTPS" certificate on the local development machine

# Requirements

- Docker - "https://www.docker.com/"
- mkcert - "https://github.com/FiloSottile/mkcert"

# Setup

```
 cd docker-wordpress-boilerplate && docker-compose up. 
```

### Access the site using the domain name
- Add the "127.0.0.1  docker-worpress-boilerplate" line to the "/etc/hosts" file.
- Now open your browser and try - ["http://docker-worpress-boilerplate:8080"]

### To replace the default cert files run the command below in the site directory

```
cd docker-wordpress-boilerplate/nginx && mkcert -cert-file docker-worpress-boilerplate.crt -key-file docker-worpress-boilerplate.key 
docker-worpress-boilerplate
```