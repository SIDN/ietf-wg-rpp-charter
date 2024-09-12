# Background and Problem Space

The Extensible Provisioning Protocol (EPP) was standardized ([STD69](https://datatracker.ietf.org/doc/std69/)) 
over 20 years ago to address the needs of domain name management between domain name registries and registrars.
Though EPP has served the domain name industry well, there is now a desire to have a provisioning protocol
using a REST architecture and JSON encoding. Such an architecture could take advantage of web-layer network
elements and other tooling. The recent deployment of RDAP in the domain name industry demonstrates adoption
of this type of architecture.

This evolution already started in the ccTLD space and first production deployments of this approach have already seen
adoption by both existing clients and a preferred way of integration for new registrars. 
A REST architecture may allow easier integration between registries and registrars, thus lowering the
costs for domain registration and new market entrants. 

# Objective and Scope

This working group is tasked with creating a series of specifications
to be known collectively as RESTful Provisioning Protocol (RPP).
These specifications will specifically target a REST architecture high on the Richardson Maturity Model
using HTTPS and JSON. 

Industry experience and use cases from EPP may influence the outputs
of this working group, but direct compatibility of RPP with EPP is not
a goal. Likewise, extensions or other changes for EPP are out of scope
of this working group. The group shall consider and enable migration scenarios
from using EPP to RPP for both clients and servers.

# Deliverables

This working group will publish on its wiki its operational practices,
including but not limited to, the adoption of work items, usage of
tools beyond the IETF’s datatracker, and implementation requirements
for the promotion of work to the IESG.

This working group will find consensus on a set of core requirements for RPP.
In alignment with the IESG's Statement on Support Documents dated 2023-08-24,
these requirements will be publicly available on the working group's wiki.
Once established, these requirements may be changed through explicit working group
consensus and in consultation with the group’s responsible Area Director.

# Milestones

After finding consensus regarding requirements, the first document to be 
delivered to the IESG by this working group will describe the core architecture of RPP with regard to the
provisioning of domain names, followed by any specifications necessary
to implement the core architecture and the JSON mapping for the different objects to be provisioned.
