**Keywords in Nginx:**

### **Global Directives**
1. **user**: Specifies the user and group for worker processes.
2. **worker_processes**: Defines the number of worker processes.
3. **worker_cpu_affinity**: Binds worker processes to specific CPU cores.
4. **worker_rlimit_nofile**: Sets the maximum number of open file descriptors.
5. **error_log**: Defines the location of the error log file.
6. **pid**: Specifies the location of the PID file.
7. **events**: Configures the event model and settings.
8. **worker_connections**: Defines the maximum number of simultaneous connections that can be handled by each worker process.
9. **multi_accept**: Determines whether a worker process accepts multiple connections at once.
### **HTTP Block Directives**
1. **http**: The main HTTP block that contains HTTP-related configurations.
2. **include**: Includes additional configuration files.
3. **server**: Defines a server block (virtual host).
4. **listen**: Specifies the address and port for a server block to listen on.
5. **server_name**: Defines the server's domain name or IP address.
6. **root**: Specifies the root directory for the server block.
7. **index**: Defines the index file(s) for a server block.
8. **access_log**: Specifies the access log file location.
9. **error_page**: Defines custom error pages.
10. **location**: Defines how requests are handled based on URI patterns.
11. **try_files**: Tries multiple files in a sequence if the requested file doesn't exist.
12. **rewrite**: Allows rewriting of URLs based on regular expressions.
13. **set**: Sets a variable.
14. **return**: Sends an HTTP response with a specified status code.
15. **add_header**: Adds headers to the response.
16. **proxy_pass**: Passes a request to a proxied server.
17. **proxy_set_header**: Modifies headers when proxying requests.
18. **fastcgi_pass**: Passes a request to a FastCGI server.
19. **uwsgi_pass**: Passes a request to a uWSGI server.
20. **limit_req**: Limits the request rate.
21. **limit_conn**: Limits the number of concurrent connections per IP.
22. **expires**: Defines expiration times for caching.
23. **gzip**: Enables or disables Gzip compression.
24. **tcp_nopush**: Optimizes network performance for certain responses.
25. **tcp_nodelay**: Disables Nagle's algorithm for improved latency in certain situations.
### **Server Block Directives**
1. **listen**: Specifies a port or address for the server to listen on.
2. **server_name**: Defines domain names or IP addresses for the server block.
3. **location**: Specifies a location block for a particular URI.
4. **root**: Defines the root directory for the server block.
5. **index**: Defines the default index files.
6. **error_page**: Specifies error handling for particular HTTP status codes.
7. **ssl_certificate**: Specifies the path to the SSL certificate.
8. **ssl_certificate_key**: Specifies the path to the SSL private key.
9. **ssl_protocols**: Defines supported SSL protocols.
10. **ssl_ciphers**: Specifies the ciphers for SSL/TLS connections.
11. **ssl_session_cache**: Configures SSL session caching.
12. **listen [IP]:[port]**: Allows binding to a specific IP address and port.
### **Location Block Directives**
1. **location**: Used to define a URI-based block for handling specific requests.
2. **alias**: Defines a file system path for a location block.
3. **proxy_pass**: Passes requests to a backend server or service.
4. **rewrite**: Modifies the URL based on a regex.
5. **try_files**: Attempts to serve different files based on conditions.
6. **return**: Sends a response with a specific HTTP status code.
7. **limit_req_zone**: Defines request rate limiting based on a shared memory zone.
### **Upstream Block Directives**
1. **upstream**: Defines an upstream server group for load balancing.
2. **server**: Defines a server in the upstream group.
3. **weight**: Assigns weight to a server in the upstream group.
4. **max_fails**: Defines the number of failed attempts before considering a server down.
5. **fail_timeout**: Specifies the period during which max_fails applies.
6. **keepalive**: Defines a maximum number of idle keepalive connections to upstream servers.
### **SSL/TLS Directives**
1. **ssl**: Enables SSL/TLS for a server block.
2. **ssl_certificate**: Specifies the SSL certificate.
3. **ssl_certificate_key**: Specifies the private key for the SSL certificate.
4. **ssl_protocols**: Defines which SSL/TLS protocols are allowed.
5. **ssl_ciphers**: Specifies the ciphers used for SSL/TLS.
6. **ssl_prefer_server_ciphers**: Configures server-side preference for SSL/TLS cipher suites.
7. **ssl_session_cache**: Configures the cache for SSL sessions.
8. **ssl_session_timeout**: Defines how long SSL session data is cached.
### **Miscellaneous Directives**
1. **include**: Includes additional configuration files into the current block.
2. **env**: Defines an environment variable for worker processes.
3. **log_format**: Defines the format for the log entries.
4. **access_log**: Specifies the file where access logs are written.
5. **client_max_body_size**: Limits the size of the body of a client request.
6. **client_body_timeout**: Defines the maximum time a client can send data.
7. **send_timeout**: Specifies the maximum time the server will take to send data to the client.
8. **connection_pool_size**: Specifies the number of connections to upstream servers.
9. **server_tokens**: Controls whether NGINX sends version information in HTTP headers.
