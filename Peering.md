
In computer networking, peering is a voluntary interconnection of administratively separate Internet networks for the purpose of exchanging traffic between the users of each network. The pure definition of peering is settlement-free, also known as "bill-and-keep," or "sender keeps all," meaning that neither party pays the other in association with the exchange of traffic; instead, each derives and retains revenue from its own customers.

## Direct Peering



[Direct Peering](https://cloud.google.com/network-connectivity/docs/direct-peering) enables you to establish a direct [peering](https://www.wikipedia.org/wiki/Peering) connection between your business network and Google's edge network and exchange high-throughput cloud traffic.

Direct Peering exists outside of Google Cloud. 

Unless you need to access Google Workspace applications, the recommended methods of access to Google Cloud are [Dedicated Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/dedicated-overview) or [Partner Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview).

Direct Peering is a good option if you already have a footprint in one of Google’s POPs—or you’re willing to lease co-location space and install and support routing equipment.

In this configuration, you run BGP over a link to exchange network routes. All traffic destined to Google rides over this new link, while traffic to other sites on the internet rides your regular internet connection.

## Carrier Peering

[Carrier Peering](https://cloud.google.com/network-connectivity/docs/carrier-peering) enables you to access Google applications, such as Google Workspace, by using a [service provider](https://cloud.google.com/network-connectivity/docs/carrier-peering#service-providers) to obtain enterprise-grade network services that connect your infrastructure to Google.


Carrier Peering is useful if installing equipment isn’t an option or you would prefer to work with a service provider partner as an intermediary to peer with Google, then Carrier Peering is the way to go.

In this configuration, you connect to Google via a new link connection that you install to a partner carrier that is already connected to the Google network itself.

You will run BGP or use static routing over that link. All traffic destined to Google rides over this new link. Traffic to other sites on the internet rides your regular internet connection.