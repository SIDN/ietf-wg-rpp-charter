# Background and Problem Space

The Extensible Provisioning Protocol (EPP) was standardized ([STD69](https://datatracker.ietf.org/doc/std69/)) 
in 2009 to address the needs of domain name management between domain name registries and registrars.
Though EPP is still serving the domain name industry well, the progress in available development, integration and operational
patterns, tools and technologies create a desire to have a provisioning protocol using the 
[REST](https://ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm) architectural style and the 
[JSON](https://datatracker.ietf.org/doc/html/rfc8259) data-interchange format. Such design is expected to 
take advantage of stateless architecture and widely deployed solutions such as OpenAPI, associated documentation,
testing and code generation tools, and L4-L7 network services such as API gateways, authorization servers, load balancers, 
web servers, WAFs etc. The successful adoption of RDAP by Domain Name Registries (DNRs) and Regional Internet Registries (RIRs) 
demonstrates the usefulness of this type of architecture and technology tool stack.

This evolution has already started with some Country Code Top Level Domains (ccTLDs). First production deployments of this approach have seen
adoption by both new and existing clients, where a preference has been noted for this approach.
A REST architecture is expected to allow easier integration between registries and registrars, thus lowering the
costs for domain registration and new market entrants.

# Objective and Scope

This working group is tasked with creating a series of specifications
to be known collectively as the RESTful Provisioning Protocol (RPP).
These specifications will specifically target a REST architecture high on the Richardson Maturity Model
using HTTPS and JSON. 

In addition to use cases, scenarios, and extension mechanisms for domain name registration, this working group will
consider features and extension mechanisms useful for other types of Internet registration areas
(e.g. IP addresses and autonomous system numbers). 

Industry experience of the ccTLDs with non-EPP provisioning protocols and use cases from EPP may influence the outputs
of this working group, but direct compatibility of RPP with EPP is not a goal.

This working group will consider functional equivalents of functionality 
from EPP for domain names, hosts and contacts ([RFC5730](https://datatracker.ietf.org/doc/html/rfc5730),
[5731](https://datatracker.ietf.org/doc/html/rfc5731), [5732](https://datatracker.ietf.org/doc/html/rfc5732), and
[5733](https://datatracker.ietf.org/doc/html/rfc5733)) and mappings for data objects, operations, commands and response.
This working group will also consider functional equivalents of registered EPP extensions, either through 
similar RPP extensions or incorporating them into the core of the protocol.
New functionalities, not having any equivalents in EPP, may be defined for RPP.

The RPP working group is focused on designing a new protocol intended to co-exist alongside EPP, 
supporting diverse needs in the ecosystem. As such, considerations for replacing EPP or migration 
scenarios away from EPP are outside the scope of this work.

The REGEXT working group is chartered to maintain and standardize extensions to EPP. Consequently, 
any extensions or changes to EPP, including those related to RPP functionality that do not exist in EPP, 
are explicitly out of scope for the RPP working group. Some IETF participants active in the REGEXT
working group will be involved in RPP working group, and coordination between the two
groups is expected.

[BCP 56](https://datatracker.ietf.org/doc/html/rfc9205) will be used to guide the specification of RPP,
and the working group may evaluate the usage of URI and HTTP specifications such as 
[RFC 6570](https://datatracker.ietf.org/doc/html/rfc6570), [RFC 8288](https://datatracker.ietf.org/doc/html/rfc8288),
[RFC 9421](https://datatracker.ietf.org/doc/html/rfc9421), [RFC 9652](https://www.rfc-editor.org/rfc/rfc9652.html), 
and the outputs of the [httpapi working group](https://datatracker.ietf.org/wg/httpapi/about/).

# Deliverables

This working group will publish on its wiki its operational practices,
including but not limited to, the adoption of work items, usage of
tools beyond the IETF’s datatracker, and implementation requirements
for the promotion of work to the IESG.

This working group will find consensus on a set of core requirements for RPP.
In alignment with the [IESG's Statement on Support Documents dated 2023-08-24](https://datatracker.ietf.org/doc/statement-iesg-support-documents-in-ietf-working-groups-20230824/),
these requirements will be publicly available on the working group's wiki.
Analysis of the functionality included and commonly used in core EPP for domain names, 
hosts and contacts ([RFC5730](https://datatracker.ietf.org/doc/html/rfc5730),
[5731](https://datatracker.ietf.org/doc/html/rfc5731), [5732](https://datatracker.ietf.org/doc/html/rfc5732), and
[5733](https://datatracker.ietf.org/doc/html/rfc5733)) is expected to be created as input material for the requirements. 
The working group may also consider RPP extensions that are functional equivalents of 
registered [EPP extensions](https://www.iana.org/assignments/epp-extensions/epp-extensions.xhtml) in
the construction of requirements.

Once established, these requirements may be changed through explicit working group 
consensus and, when the chairs determine it to be a major change, in consultation 
with the group’s responsible Area Director. The finding of consensus for both the 
initial requirements and any changes will be explicitly noted by the chairs on the 
working group's mailing list.

After finding consensus regarding requirements, the working group will deliver to the
IESG documents addressing the following topics in an order determined through agreement
of the chairs with the responsible Area Director:
* core architecture, including extension mechanisms
* specifications necessary to implement the core architecture
* specifications necessary to implement extensions
* specifications regarding the provisioning of domain names using RPP
* mappings between RPP and EPP

The working group may consider work for the provisioning of other types of Internet registries (e.g. IP addresses
and autonomous system numbers) with consultation from the responsible Area Director.

A written record of acceptance with an explanation of working group scope of I-Ds as working group work items 
is to be recorded with explicit acknowledgement of the chairs and published on the wiki.

