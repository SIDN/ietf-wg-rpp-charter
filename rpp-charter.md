# Background and Problem Space

The Extensible Provisioning Protocol (EPP) was standardized ([STD69](https://datatracker.ietf.org/doc/std69/)) 
over 20 years ago to address the needs of domain name management between domain name registries and registrars.
EPP has served the domain name industry well, but despite its extensibility features 
it is not well-suited for RESTful environments that take advantage of web-layer firewalls and load-balancers,
serverless-oriented computing, and other tools tailored to RESTful protocols. 

EPP is primarily used in the domain name industry, and there is a growing 
need from regional Internet registries (RIRs) for a common unified protocol in the provisioning of IP addresses and ASNs. 
RIRs have developed their own RESTful provisioning APIs and EPP cannot fulfill their needs as a good starting point 
for a unified approach as it is not RESTful. 

There is a desire to create a new domain name provisioning protocol based on state-of-the-art RESTful principles 
and corresponding data representations using JSON instead of XML. The protocol will specifically target modern, RESTful
tooling for the construction of software as well as scalable infrastructure as is commonly found in cloud 
and on-premises stateless, serverless, container and virtual application clustering technologies.

This evolution already started in ccTLD space and first production deployments of this approach already proved 
very good adoption by both existing clients as well as a preferred way of integration for the new registrants. 
The use of RESTful principles allows for easier integration with registry functions, enabling smaller registrars 
to also leverage the automated provisioning channel.

# Objective and Scope

This working group is tasked with creating a series of specifications
to be known collectively as RESTful Provisioning Protocol (RPP).
These specifications will specifically target RESTful software development methodologies as well as 
scalable infrastructure as is commonly found in cloud and on-premises stateless, serverless, containerized and 
virtual application clustering technologies.


Industry experience and use cases from EPP may influence the outputs
of this working group, but direct compatibility of RPP with EPP is not
a goal. Likewise, extensions or other changes for EPP are out of scope
of this working group.

TODO: mention no support for XML?

# Deliverables

After the timely delivery of the core set of RPP specifications and in
consultation with the working group’s responsible Area Director, this
working group may consider work on enabling technologies for the
unilateral and/or multilateral flow of provisioning work between RPP
and EPP given the proviso above regarding changes to EPP.

This working group will publish on its wiki its operational practices,
including but not limited to, the adoption of work items, usage of
tools beyond the IETF’s datatracker, and implementation requirements
for the promotion of work to the IESG.

This working group will also establish a set of core requirements for
RPP to be published on the working group’s wiki. Once established,
these requirements may be changed through explicit working group
consensus and in consultation with the group’s responsible Area
Director.

# Milestones

The first document to be delivered to the IESG by this working group
will describe the core architecture of RPP with regard to the
provisioning of domain names, followed by any specifications necessary
to implement the core architecture and the JSON mapping for the different objects to be provisioned.
