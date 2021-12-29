## Cloud CDN

[Cloud CDN](https://cloud.google.com/cdn/) (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs.

https://cloud.google.com/cdn/docs/overview


### Using CDN with backend bucket

https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket


### Using CDN with managed instance group

https://cloud.google.com/cdn/docs/setting-up-cdn-with-mig


### Using CDN with an external origin

https://cloud.google.com/cdn/docs/setting-up-cdn-with-external-origin


## HTTP/3 

HTTP/3 is a next-generation internet protocol, and is built on top of [QUIC](https://datatracker.ietf.org/doc/html/rfc9000).

HTTP/3 can [work with Cloud CDN and Load Balancing](https://cloud.google.com/blog/products/networking/cloud-cdn-and-load-balancing-support-http3).

## External HTTP(S) Load Balancing

Cloud CDN works with external HTTP(S) Load Balancing to deliver content to your users. The external HTTP(S) load balancer provides the frontend IP addresses and ports that receive requests and the backends (or origins) that respond to the requests.

https://cloud.google.com/cdn/docs/using-cdn

## Types of CDN

CDN is an umbrella term spanning different types of content delivery services: video streaming, software downloads, web and mobile content acceleration, licensed/managed CDN, transparent caching, and services to measure CDN performance, load balancing, Multi CDN switching and analytics, and cloud intelligence. CDN vendors may cross over into other industries like security, with [DDoS](DDoS) protection and web application firewalls (WAF), and WAN optimization.

https://blog.cdnsun.com/how-to-compare-cdn-networks-a-pro-guide/

https://cdncomparison.com/

https://wikipedia.org/wiki/Content_delivery_network


## CDN, DNS and Anycast

https://blog.cdnsun.com/understanding-cdn-dns-routing-unicast-versus-anycast/
