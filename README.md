# Nginx PHP

Nginx server that can run simple PHP scripts.

## Getting started

### Test domain

On Windows, add this to your `hosts` file.

    127.0.0.1 php-site.local

### Create docker network

Check whether you have the `nginx-proxy` network.

    docker network ls

If not found, create the `nginx-proxy` network.

    docker network create nginx-proxy

### Start the container

Start the container

    docker compose up -d

You can then access the application through the following URLs:

    http://127.0.0.1:8088/
    http://127.0.0.1:8088/foobar.php

OR

    http://php-site.local
    http://php-site.local/foobar.php
