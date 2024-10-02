Nginx is a popular open-source web server software that can also function as a reverse proxy, load balancer, mail proxy and HTTP cache. Here are the key points about Nginx:

### What is Nginx?

- Nginx (pronounced "engine-x") is a web server that was originally created to solve the C10k problem (handling 10,000 concurrent connections).

- It was developed by Igor Sysoev and first publicly released in 2004.

- Nginx is free and open-source software, released under the BSD license.

### Key Features and Capabilities

- Web server - Can serve static web content efficiently.

- Reverse proxy - Can act as an intermediary for client requests to backend servers.

- Load balancer - Can distribute traffic across multiple servers.

- HTTP cache - Can cache content to improve performance.

- Mail proxy.

### How Nginx Works

- Uses an asynchronous, event-driven approach to handle requests.

- Has a master process that manages multiple worker processes.

- Can handle thousands of concurrent connections efficiently.

- Modular architecture allows for extending functionality.

### Popularity and Usage

- As of June 2022, Nginx was used by 33.6% of all websites.

- Particularly popular among high-traffic websites.

- Used by major companies like Netflix, NASA, WordPress.com and many others.

### Comparison to Apache

- Nginx is often considered to have better performance under high loads compared to Apache.

- Nginx is more popular among high-traffic sites, while Apache has higher overall usage.

In summary, Nginx is a versatile and high-performance web server software that excels at handling concurrent connections and is widely used for serving web content, load balancing, and as a reverse proxy.



# feature of nginx
- caching
- load balancing
- security
- encrypted communication
- compression - use less intenet bandwidth

# configure nginx
- directives
	- configure load balancing algorithm
	- 