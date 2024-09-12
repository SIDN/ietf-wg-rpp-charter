# Background and Motivation
The Extensible Provisioning Protocol (EPP) was standardized (STD69) over 20 years ago to address the needs of domain name management between domain name registries and registrars. It encodes protocol Request and response using XML and can be carried over multiple transport protocols. Though EPP has served the domain name industry well, there is now a desire to modernize provisioning protocol using a RESTFUL design and JSON encoding. Such design could take advantage of stateless architecture and widely deployed tooling such as POSTMAN, SWAGGER. 

The recent deployment of Registration Data Access Protocol(RDAP RFCs 7480-7484) in the domain name industry demonstrates the need of evolution toward this type of architecture.
For example, this evolution has already started in the ccTLD space and first production deployments of this approach have already been adopted by both existing registrars and new registrars as a preferred way of integration for the latter one. A REST architecture may allow easier integration between registries and registrars, thus lowering the costs for domain registration.

# Objective and Scope
The RPP Working Group is chartered to develop a series of specifications to be known collectively as RESTful Provisioning Protocol (RPP). These specifications will specifically target a REST architecture using HTTPS and JSON. The Working Group will concentrate on the following:
o Collecting and documenting a set of core requirements for RPP. These requirements will be publicly available on the working group's wiki.
o Developing RPP Architecture for the provisioning of domain names. It Supports RPP transport over HTTPS and Encode protocol Request and response with JSON.
o Providing RPP Domain Name JSON Mapping for the different objects to be provisioned.

# Out of Scope
Industry experience and use cases from EPP may influence the outputs of this working group, but direct compatibility of RPP with EPP is not a goal. Likewise, extensions or other changes for EPP are out of scope of this working group.

# Work items
The RPP Working Group will initially focus on the following deliverables:
o wiki or internet draft for core requirements for RPP.
o Standard Track document for RPP architecture (1)provide a standard Internet domain name registration protocol for use between domain
   name registrars and domain name registries. (2)Support RPP transport over HTTPS (3) Encode protocol Request and response with JSON
o Standard Track document for RPP Domain Name JSON Mapping to provide Internet domain name mapping for RPP protocol.

This working group will find consensus on a set of core requirements for RPP. In alignment with the IESG's Statement on Support Documents dated 2023-08-24, these requirements will be publicly available on the working group's wiki. Once established, these requirements may be changed through explicit working group consensus and in consultation with the group’s responsible Area Director.

# Dependencies and Liaisons
The GREEN Working Group will closely collaborate with REGEXT WG that addresses topics related to EPP and RDAP use.
