https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0

# ClusterIP
A ClusterIP service is the default Kubernetes service. It gives you a service inside your cluster that other apps inside your cluster can access. There is no external access.

# NodePort
A NodePort service is the most primitive way to get external traffic directly to your service. NodePort, as the name implies, opens a specific port on all the Nodes (the VMs), and any traffic that is sent to this port is forwarded to the service.

# LoadBalancer
A LoadBalancer service is the standard way to expose a service to the internet. On GKE, this will spin up a [Network Load Balancer\(https://cloud.google.com/compute/docs/load-balancing/network/) that will give you a single IP address that will forward all traffic to your service.

# Ingress

Ingress
Unlike all the above examples, Ingress is actually NOT a type of service. Instead, it sits in front of multiple services and act as a “smart router” or entrypoint into your cluster.

You can do a lot of different things with an Ingress, and there are many types of Ingress controllers that have different capabilities.
The default GKE ingress controller will spin up a [HTTP(S) Load Balancer](https://cloud.google.com/compute/docs/load-balancing/http/) for you. This will let you do both path based and subdomain based routing to backend services. For example, you can send everything on foo.yourdomain.com to the foo service, and everything under the yourdomain.com/bar/ path to the bar service.


https://kubernetes.io/docs/concepts/services-networking/ingress/

 You can deploy other [Ingress controllers](https://kind.sigs.k8s.io/docs/user/ingress/#using-ingress). The following [ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/) controllers are widely used:

* [Ambassador](https://kind.sigs.k8s.io/docs/user/ingress/#ambassador)   https://www.getambassador.io/
* [Contour](https://kind.sigs.k8s.io/docs/user/ingress/#contour)  https://projectcontour.io/
* [Ingress NGINX](https://kind.sigs.k8s.io/docs/user/ingress/#ingress-nginx) https://www.nginx.com/products/nginx-ingress-controller/


