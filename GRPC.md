

gRPC is a technology for implementing RPC APIs that uses HTTP 2.0 as its underlying transport protocol. 

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



