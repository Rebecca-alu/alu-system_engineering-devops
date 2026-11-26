# Load balancer

- `0-custom_http_response_header` - Installs Nginx and adds the X-Served-By header with the server's hostname
- `1-install_load_balancer` - Installs HAProxy and sends traffic to web-01 and web-02 with roundrobin
