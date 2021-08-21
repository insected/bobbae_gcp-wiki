

[gRPC](https://grpc.io/) is a technology for implementing RPC APIs that uses HTTP 2.0 as its underlying transport protocol. 


GRPC is a high performance, open-source universal RPC framework, developed by Google. In gRPC, a client application can directly call methods on a server application on a different machine as if it was a local object, making it easier to create distributed applications and services.

One of the primary benefits of using gRPC is for documentation; you can use your service configuration and API interface definition files to generate reference documentation for your API. 

With [Endpoints for gRPC](https://cloud.google.com/endpoints/docs/grpc/about-grpc), you can use the API management capabilities of [Endpoints](Endpoints) to add an API console, monitoring, hosting, tracing, authentication, and more to your gRPC services. In addition, once you specify special mapping rules, ESP and ESPv2 translate [RESTful](https://en.wikipedia.org/wiki/Representational_state_transfer) JSON over HTTP into gRPC requests. This means that you can deploy a gRPC server managed by Endpoints and call its API using a gRPC or JSON/HTTP client, giving you much more flexibility and ease of integration with other systems.


https://cloud.google.com/endpoints/docs/grpc/about-grpc


## REST

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000 in [his famous dissertation](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm).

https://restfulapi.net/

The key abstraction of information in REST is a resource. Any information that can be named can be a resource: a document or image, a temporal service, a collection of other resources, a non-virtual object (e.g. a person), and so on. REST uses a resource identifier to identify the particular resource involved in an interaction between components.



https://en.wikipedia.org/wiki/Representational_state_transfer

## gRPC

A second model for using HTTP for APIs is illustrated by gRPC. gRPC uses HTTP/2 under the covers, but HTTP is not exposed to the API designer. gRPC-generated stubs and skeletons hide HTTP from the client and server too, so nobody has to worry how the RPC concepts are mapped to HTTP—they just have to learn gRPC. 

The way a client uses a gRPC API is by following these three steps:

- Decide which procedure to call

- Calculate the parameter values to use (if any)

- Use a code-generated stub to make the call, passing the parameter values

### Quickstart in Go

https://grpc.io/docs/languages/go/quickstart/

### Remote Procedure Call

In distributed computing, a remote procedure call (RPC) is when a computer program causes a procedure (subroutine) to execute in a different address space (commonly on another computer on a shared network), which is coded as if it were a normal (local) procedure call, without the programmer explicitly coding the details for the remote interaction. That is, the programmer writes essentially the same code whether the subroutine is local to the executing program, or remote.

https://en.wikipedia.org/wiki/Remote_procedure_call

## Protocol Buffers


Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler. You define how you want your data to be structured once, then you can use special generated source code to easily write and read structured data to and from a variety of data streams and using a variety of languages.

https://developers.google.com/protocol-buffers/

### Thrift, XDR, Avro, MessagePack, BSON, etc.

https://www.igvita.com/2011/08/01/protocol-buffers-avro-thrift-messagepack/

https://en.wikipedia.org/wiki/External_Data_Representation

https://stellar.stackexchange.com/questions/271/why-did-the-project-settle-on-xdr-for-external-data-serialisation


## When to use REST vs. gRPC

https://cloud.google.com/blog/products/api-management/understanding-grpc-openapi-and-rest-and-when-to-use-them


## GRPC Endpoints Tutorials

https://cloud.google.com/endpoints/docs/grpc/tutorials

## Python GRPC Microservices

https://realpython.com/python-microservices-grpc/

