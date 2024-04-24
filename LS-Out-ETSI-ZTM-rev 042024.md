We would like to thank the ETSI ISG ZSM for informing us [1] about the initiation
of a new normative specification work on Network Digital Twin "ETSI GS ZSM018 Network
Digital Twin for enhanced zero-touch network and service management".

For your information, the IETF has chartered a new Working Group (WG) on Network Management
OPerations (NMOP WG) [2]. One of the current NMOP WG topics is investigating issues
related to the deployment and usage of YANG topology modules in order to model a Digital Map.

Specifically, the WG is discussing "Modeling the Digital Map based on RFC 8345: Sharing Experience
and Perspectives” [3] which defines the concept of Digital Map and explains its connection to the 
Network Digital Twin (NDT). Also, the document identifies a set of candidate issues in RFC 8345 to
meet NDT needed. These issues will be fixed as part of the NMOP WG activities.

The Digital Map effort leverages the NDT architecture defined in the IRTF “Network Digital Twin: Concepts and
Reference Architecture” [4] specification which also provides an overview of the NDT terms and
concepts.

In addition, the ongoing effort leverages existing tools and data models, such as (but not limited to):

* A "Framework for Automating Service and Network Management with YANG" [5] describes a framework
  for service and network management automation that takes advantage of YANG modeling technologies.

    + This framework is drawn irrespective of the origin of a data model; thus, it can accommodate YANG
  modules that are developed outside the IETF.
    + Data models are also instrumental in the automation of network management, and they can provide
    closed-loop control for adaptive and deterministic service creation, delivery, and maintenance.

* YANG is a data modeling language that is independent of both the encoding and the transport that is used. Many of the YANG modules are used to
  exchange data between NETCONF/RESTCONF clients and servers ([RFC 6241](https://datatracker.ietf.org/doc/html/rfc6241), [RFC 8040](https://datatracker.ietf.org/doc/html/rfc8040)). However, YANG can be used by encodings other than XML/JSON and protocols other than NETCONF/RESTCONF.

*	The IETF has specified a comprehensive list of models which cover various layers and components. For example:

 	 + Service-level abstractions to represent how a service is exposed by a network to a customer:

       - [RFC 8309](https://datatracker.ietf.org/doc/html/rfc8309): Service Models Explained
       - [RFC 8299](https://datatracker.ietf.org/doc/html/rfc8299): The L3VPN Service Model
       - [RFC 8466](https://datatracker.ietf.org/doc/html/rfc8466): The L2VPN Service Model
         
   + Network-level abstractions, including devices and their subsystems, and relevant protocols operating at the link and network
     layers across multiple devices. Examples of such models are as follows:
     
       - [RFC 8345](https://datatracker.ietf.org/doc/html/rfc8345): The Network Topologies Model defines a base model for network topology
         and inventories. Network topology data includes link, node, and terminate-point resources.
       - [RFC 8795](https://datatracker.ietf.org/doc/html/rfc8795): The TE Topology Model defines a YANG data model for representing and manipulating TE topologies.
       - [RFC 8346](https://datatracker.ietf.org/doc/html/rfc8346): The Layer 3 Topology Model defines a YANG data model for representing and manipulating Layer 3 topologies.
       - [RFC 8944](https://datatracker.ietf.org/doc/html/rfc8944): The Layer 2 Topology Model defines a YANG data model for representing and manipulating Layer 2 topologies.
       - [RFC 8675](https://datatracker.ietf.org/doc/html/rfc8675): defines a collection of YANG identities used as interface types for tunnel interfaces.
       - [RFC 9182](https://datatracker.ietf.org/doc/html/rfc9182): The L3VPN Network Model (L3NM) provides a network-centric view of L3VPN services within a network.
       - [RFC 9291](https://datatracker.ietf.org/doc/html/rfc9291): The L2VPN Network Model (L2NM) provides a network-centric view of L2VPN services within a network.
       - [RFC 9408](https://datatracker.ietf.org/doc/html/rfc9408): The Service Access Point (SAP) model defines a YANG data model for representing an abstract view
         of the provider network topology that contains the points from which its services can be attached
         (e.g., basic connectivity, VPN, Network Slices).

   + Sample device models:
     
      - [RFC 8530](https://datatracker.ietf.org/doc/html/rfc8530): The Logical Network Element Model defines a logical network element model that
        can be used to manage the logical resource partitioning that may be present on a network
        device.
      - [RFC 8529](https://datatracker.ietf.org/doc/html/rfc8529): The Network Instance Model defines a network instance module. This module can
        be used to manage the virtual resource partitioning that may be present on a network device.
      - [RFC 8348](https://datatracker.ietf.org/doc/html/rfc8348): defines a YANG module for the management of hardware.
      - [RFC 7317](https://datatracker.ietf.org/doc/html/rfc7317): defines the "ietf-system" YANG module that provides many features such as
        the configuration and the monitoring of system or system control operations
        (e.g., shutdown, restart, and setting time) identification.
      - [RFC 8341](https://datatracker.ietf.org/doc/html/rfc8341): defines a network configuration access control YANG module.
      - [RFC 7224](https://datatracker.ietf.org/doc/html/rfc7224): defines a YANG module for interface type definitions.
      - [RFC 8343](https://datatracker.ietf.org/doc/html/rfc8343): defines a YANG module for the management of network interfaces.
      - [RFC 8349](https://datatracker.ietf.org/doc/html/rfc8349): defines a YANG module for routing management.
      - [RFC 8512](https://datatracker.ietf.org/doc/html/rfc8512): defines a YANG module for NAT management.
      - [RFC 8519](https://datatracker.ietf.org/doc/html/rfc8519): defines a YANG module for managing Access Control Lists.
      - …
        
  * Available data models can be retrieved from [6].

The NMOP WG believes that existing data models can be leveraged in the context of NDT beyond the IETF.
Concretely, the Digital Map is a key foundation for building the NDT, independent of the applications
that will use this NDT.

The NMOP WG encourages the use of NMOP WG mailing list [7] as the most effective and expedient
way of exchanging information, answering questions, and progressing any work. The WG will consider
presentation requests from the ETSI ISG ZSM that describe data modeling issues that you may identify,
including, but not limited to, when integrating and consuming existing data models. Such issues
can also be shared during formal WG meetings. Requests for presentations can be sent to the NMOP Chairs [8].

Following is the schedule of upcoming IETF meetings [9]:

* 20 July 2024 - 26 July 2024, Vancouver Canada
* 02 Nov 2024 - 08 Nov 2024, Dublin Ireland

NMOP Chairs

Mohamed Boucadair & Benoît Claise


* [1] https://datatracker.ietf.org/liaison/1914/ 
* [2] https://datatracker.ietf.org/group/nmop/about/
* [3] https://datatracker.ietf.org/doc/draft-havel-nmop-digital-map/
* [4] https://datatracker.ietf.org/doc/draft-irtf-nmrg-network-digital-twin-arch/
* [5] https://datatracker.ietf.org/doc/html/rfc8969
* [6] https://www.yangcatalog.org/yang-search
* [7] https://www.ietf.org/mailman/listinfo/nmop
* [8] nmop-chairs@ietf.org
* [9] https://www.ietf.org/meeting/upcoming/
* RFCs cited in the LS can be retrieved from https://datatracker.ietf.org/
