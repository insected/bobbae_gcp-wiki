

[gRPC](https://grpc.io/) is a technology for implementing [RPC](http://dist-prog-book.com/chapter/1/rpc.html) APIs that uses HTTP 2.0 as its underlying transport protocol. 


gRPC is a high performance, open-source [universal RPC framework](https://github.com/grpc-ecosystem/awesome-grpc), developed by Google. In gRPC, a client application can directly call methods on a server application on a different machine as if it was a local object, making it easier to create distributed applications and [micro services](https://github.com/mfornos/awesome-microservices).

One of the primary benefits of using gRPC is for documentation; you can use your service configuration and API interface definition files to generate reference documentation for your API. 

With [Google Endpoints for gRPC](https://cloud.google.com/endpoints/docs/grpc/about-grpc), you can use the API management capabilities of [Google Endpoints](Endpoints) to add an API console, monitoring, hosting, tracing, authentication, and more to your gRPC services. In addition, once you specify special mapping rules, ESP and ESPv2 translate [RESTful](https://en.wikipedia.org/wiki/Representational_state_transfer) JSON over HTTP into gRPC requests. This means that you can deploy a gRPC server managed by Endpoints and call its API using a gRPC or JSON/HTTP client, giving you much more flexibility and ease of integration with other systems.


https://cloud.google.com/endpoints/docs/grpc/about-grpc


## REST

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000 in [his famous dissertation](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm).

https://restfulapi.net/

The key abstraction of information in REST is a resource. Any information that can be named can be a resource: a document or image, a temporal service, a collection of other resources, a non-virtual object (e.g. a person), and so on. REST uses a resource identifier to identify the particular resource involved in an interaction between components.



https://en.wikipedia.org/wiki/Representational_state_transfer

It provides operations (HTTP methods) such as GET, POST, PUT, and DELETE. By using a [stateless](https://restfulapi.net/statelessness/) protocol and standard operations, RESTful systems aim for fast performance, reliability, and the ability to grow by reusing components that can be managed and updated without affecting the system as a whole, even while it is running.


## gRPC

gRPC uses HTTP/2 under the covers, but HTTP is not exposed to the API designer. gRPC-generated stubs and skeletons hide HTTP from the client and server too, so nobody has to worry how the RPC concepts are mapped to HTTP???they just have to learn gRPC. 



### gRPC vs REST

https://blog.dreamfactory.com/grpc-vs-rest-how-does-grpc-compare-with-traditional-rest-apis/

https://cloud.google.com/blog/products/api-management/understanding-grpc-openapi-and-rest-and-when-to-use-them

https://phil.tech/2017/rest-confusion-explained/


### Quickstart in Go

https://grpc.io/docs/languages/go/quickstart/

### Remote Procedure Call

In distributed computing, a remote procedure call (RPC) is when a computer program causes a procedure (subroutine) to execute in a different address space (commonly on another computer on a shared network), which is coded as if it were a normal (local) procedure call, without the programmer explicitly coding the details for the remote interaction. That is, the programmer writes essentially the same code whether the subroutine is local to the executing program, or remote.

https://en.wikipedia.org/wiki/Remote_procedure_call

## Protocol Buffers


[Protocol buffers](https://developers.google.com/protocol-buffers/) are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data ??? think XML, but smaller, faster, and simpler. You define how you want your data to be structured once, then you can use special generated source code to easily write and read structured data to and from a variety of data streams and using a variety of languages.

https://developers.google.com/protocol-buffers/docs/proto3


There are [many other Data serialization formats](Data-Serialization-Formats)

### MessagePack

https://msgpack.org/

### Avro

https://avro.apache.org/

### Thrift

https://thrift.apache.org/

### Flatbuffers

https://github.com/google/flatbuffers

### Capt'n Proto

https://capnproto.org/

## When to use REST vs. gRPC

https://cloud.google.com/blog/products/api-management/understanding-grpc-openapi-and-rest-and-when-to-use-them


## gRPC Endpoints Tutorials

https://cloud.google.com/endpoints/docs/grpc/tutorials

## Python gRPC Microservices

https://realpython.com/python-microservices-grpc/

## RPC, REST and HTTP

https://www.smashingmagazine.com/2016/09/understanding-rest-and-rpc-for-http-apis/


## ALTS

https://cloud.google.com/docs/security/encryption-in-transit/application-layer-transport-security

### gRPC and Envoy


https://github.com/soeirosantos/alts-go-grpc-envoy

https://medium.com/google-cloud/grpc-application-layertransport-security-alts-helloworld-f26e4b05f329

