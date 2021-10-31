# compose-portainer

## Requirements:
* docker >= 17.12.0+
* docker-compose

## Quick Start
* Clone or download this repository
* Go inside of directory,  `cd compose-portainer`
* Run this command `docker-compose up -d`

## Access to Portainer: 

**URL:** `http://localhost:9000`

``` 
user: admin
pass: password
``` 

## Password Generation

```
docker run --rm httpd:2.4-alpine htpasswd -nbB admin 'password' | cut -d ":" -f 2 | sed 's/\$/\$\$/g'

``` 