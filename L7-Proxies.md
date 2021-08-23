

In a microservice architecture, services communicate with each other through [Layer 7](  https://en.m.wikipedia.org/wiki/Application_layer  ) protocols such as [gRPC](GRPC) and HTTP. Since the network is not reliable (and services can go down!), managing L7 communications is critical for reliability and scale.

## L7 Proxies and API Gateways

* [Traefik](https://traefik.io/)
* [NGINX](http://nginx.org/)
* [HAProxy](http://www.haproxy.org/)
* [Envoy](https://www.envoyproxy.io/)
* [Ambassador](https://getambassador.io)

## Envoy

Envoy pioneered the use of dynamic APIs for management, and an ecosystem of additional open source projects that use Envoy has evolved. These projects generally function as so-called control planes to manage Envoy. Projects that use Envoy proxy include Consul Connect, Istio, and Ambassador.

https://www.envoyproxy.io/

## Sidecar Proxy

https://blog.envoyproxy.io/introduction-to-modern-network-load-balancing-and-proxying-a57f6ff80236


## Service Mesh

A [Service Mesh](Service-Mesh) is a transparent layer that adds resilience, observability, and security to your service-to-service communication. Example service meshes include Istio and Linkerd. Istio is closely associated with Envoy because Istio relies on Envoy to do the actual Layer 7 traffic management. Istio itself is a control plane for a fleet of Envoy Proxies that are deployed next to your microservices.

