## Load Balancer

This section covers configuring Nginx response headers and installing HAProxy
to distribute HTTP traffic between two web servers.

### Tasks

**0. Custom HTTP response header**

`load_balancer/0-custom_http_response_header`

A Bash script that installs Nginx and configures the X-Served-By HTTP
response header to display the hostname of the web server.

**1. Install a load balancer**

`load_balancer/1-install_load_balancer`

A Bash script that installs and configures HAProxy to distribute HTTP
requests between two web servers using the roundrobin algorithm.

The backend servers are:

- 7423-web-01: 18.134.226.27
- 7423-web-02: 35.176.119.210
