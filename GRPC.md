As most software developers no doubt know, there are two primary models for API design: RPC and REST. Regardless of model, most modern APIs are implemented by mapping them in one way or another to the same HTTP protocol. It has also become common for RPC API designs to adopt one or two ideas from HTTP while staying within the RPC model, which has increased the range of choices that an API designer faces. This post tries to explain the choices, and give guidance on how to choose between them.

gRPC is a technology for implementing RPC APIs that uses HTTP 2.0 as its underlying transport protocol. You might expect that gRPC and HTTP would be mutually exclusive, since they are based on opposite conceptual models. gRPC is based on the Remote Procedure Call (RPC) model, in which the addressable entities are procedures, and the data is hidden behind the procedures. HTTP works the inverse way. In HTTP, the addressable entities are “data entities” (called “resources” in the HTTP specifications), and the behaviors are hidden behind the data—the behavior of the system results from creating, modifying, and deleting resources.

Most public APIs and many private distributed APIs use HTTP as the transport, at least in part because organizations are accustomed to dealing with the security issues of allowing HTTP traffic on ports 80 and 443.

In my opinion there are three significant and distinct approaches for building APIs that use HTTP. They are:

- REST

- gRPC (and Apache Thrift and others)

- OpenAPI (and its competitors)

## REST

REST
The least-commonly used API model is REST—only a small minority of APIs are designed this way, even though the word REST is used (or abused) more broadly. A signature characteristic of this style of API is that clients do not construct URLs from other information—they just use the URLs that are passed out by the server as-is. This is how the browser works—it does not construct the URLs it uses from piece parts, and it does not understand the website-specific formats of the URLs it uses; it just blindly follows the URLs that it finds in the current page received from the server, or that were bookmarked from previous pages or are entered by the user. The only parsing of a URL that a browser does is to extract the information required to send an HTTP request, and the only construction of URLs that a browser does is to form an absolute URL from relative and base URLs. If your API is a REST API, then your clients never have to understand the format of your URLs and those formats are not part of the API specification given to clients1. 

REST APIs can be very simple. Lots of additional technologies have been invented for use with REST APIs—for example JSON API, ODATA, HAL, Siren or JSON Hyper-Schema and others—but you don't need any of those to do REST well.

## gRPC

A second model for using HTTP for APIs is illustrated by gRPC. gRPC uses HTTP/2 under the covers, but HTTP is not exposed to the API designer. gRPC-generated stubs and skeletons hide HTTP from the client and server too, so nobody has to worry how the RPC concepts are mapped to HTTP—they just have to learn gRPC. 

The way a client uses a gRPC API is by following these three steps:

- Decide which procedure to call

- Calculate the parameter values to use (if any)

- Use a code-generated stub to make the call, passing the parameter values


## OpenAPI

Probably the most popular way of designing RPC APIs that use HTTP is to use specification languages like OpenAPI (formerly known as the Swagger specification).

A signature characteristic of the OpenAPI style of API is that clients use the API by constructing URLs from other information. The way a client uses an OpenAPI API is by following these three steps:

- Decide which OpenAPI URL path template to use

- Calculate the parameter values to use (if any)

- Plug the parameter values into the URL path template and send an HTTP request.

It should be immediately obvious that an API that works this way is not a REST API. The OpenAPI method of using HTTP requires clients to have detailed knowledge of the format of the URLs they use in requests and to construct URLs that conform to that format from other information. This is the opposite of the way a REST API works, where clients are completely blind to the formats of the URLs they use, and never have to construct them. The model supported by OpenAPI is very popular and successful and is one of the most important options available to API designers—the fact that the OpenAPI model is not REST does not diminish its usefulness or importance.

