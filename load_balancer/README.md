Load Balancer

Description

This project focuses on configuring Nginx web servers and setting up HAProxy as a load balancer to distribute incoming HTTP traffic between two web servers.

Tasks

0. Custom HTTP Response Header

The 0-custom_http_response_header script:

Installs Nginx.

Configures the X-Served-By HTTP response header.

Uses the server hostname as the header value.

Restarts Nginx after configuration.

1. Install Load Balancer

The 1-install_load_balancer script:

Installs HAProxy.

Configures HAProxy to listen on port 80.

Distributes traffic between two web servers using the round-robin algorithm.

Enables and restarts the HAProxy service.

Requirements

Ubuntu server

Bash

Nginx

HAProxy

Usage

Run the scripts with root privileges on their respective servers:

sudo ./0-custom_http_response_header
sudo ./1-install_load_balancer

The first script should be executed on each web server, while the second should be executed on the load balancer server.
