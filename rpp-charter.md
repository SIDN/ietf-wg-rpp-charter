# Introduction

The Extensible Provisioning Protocol (EPP) was standardized ([STD69](https://datatracker.ietf.org/doc/std69/)) in 2009 to address the needs of domain name management between domain name registries and registrars.
Though EPP is still serving the domain name industry well, the progress in available development, integration and operational patterns, tools and technologies create a desire to have a provisioning protocol using the [Representational State Transfer (REST)](https://ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm) architectural style and the [JSON](https://datatracker.ietf.org/doc/html/rfc8259) data-interchange format. 
Such design is expected to take advantage of stateless architecture and widely deployed solutions such as OpenAPI, associated documentation, testing and code generation tools, and L4-L7 network services such as API gateways, authorization servers, load balancers, web servers, web application firewalls, etc. 
The successful adoption of Registration Data Access Protocol (RDAP) by Domain Name Registries (DNRs) and Regional Internet Registries (RIRs) demonstrates the usefulness of JSON and REST based architectures.

Production deployments of REST and JSON based provisioning protocols by Country Code Top Level Domains (ccTLDs) have been well received, however variance across implementations is starting to become a concern.

A standardized REST architecture is expected to allow easier integration between registries and registrars, thus lowering the costs for domain registration and new market entrants.

# Scope

The RPP WG is tasked with creating a series of specifications to be known collectively as the RESTful Provisioning Protocol (RPP).
These specifications target a REST architecture high on the Richardson Maturity Model using HTTPS and JSON. 

In addition to use cases, scenarios, and extension mechanisms for domain name registration, the RPP WG considers features and extension mechanisms useful for other types of Internet registration areas (e.g. IP addresses and autonomous system numbers). 

The RPP WG considers functional equivalents of functionality from EPP for domain names, hosts and contacts ([RFC5730](https://datatracker.ietf.org/doc/html/rfc5730), [5731](https://datatracker.ietf.org/doc/html/rfc5731), [5732](https://datatracker.ietf.org/doc/html/rfc5732), and [5733](https://datatracker.ietf.org/doc/html/rfc5733)) and mappings for data objects, operations, commands and responses.

New functionalities, not having any equivalents in EPP or [EPP extensions](https://www.iana.org/assignments/epp-extensions/epp-extensions.xhtml), may be defined for RPP.

The RPP working group is focused on designing a new protocol intended to co-exist alongside EPP, supporting diverse needs in the ecosystem. 
As such, considerations for replacing EPP or migration scenarios away from EPP are outside the scope of the RPP WG.

The REGEXT working group is chartered to maintain and standardize extensions to EPP. 
Consequently, any extensions or changes to EPP, including those related to RPP functionality that do not exist in EPP, are explicitly out of scope for the RPP working group. 

# Working Group Process

The charter in datatracker is the source of truth for all official working group process requirements.

However, the RPP WG publishes its usage of tools beyond the datatracker and mailing lists on its wiki.

[BCP 56](https://datatracker.ietf.org/doc/html/rfc9205) is used to guide the specification of RPP, along with [RFC 6570](https://datatracker.ietf.org/doc/html/rfc6570), [RFC 8288](https://datatracker.ietf.org/doc/html/rfc8288), [RFC 9421](https://datatracker.ietf.org/doc/html/rfc9421), [RFC 9652](https://www.rfc-editor.org/rfc/rfc9652.html), and the outputs of the [httpapi working group](https://datatracker.ietf.org/wg/httpapi/about/).

Analysis of the functionality included and commonly used in core EPP for domain names, hosts and contacts ([RFC5730](https://datatracker.ietf.org/doc/html/rfc5730), [5731](https://datatracker.ietf.org/doc/html/rfc5731), [5732](https://datatracker.ietf.org/doc/html/rfc5732), and [5733](https://datatracker.ietf.org/doc/html/rfc5733)) is developed to support the deliverables. 

In alignment with the [IESG's Statement on Support Documents dated 2023-08-24](https://datatracker.ietf.org/doc/statement-iesg-support-documents-in-ietf-working-groups-20230824/), these supporting documents are publicly available on the working group's wiki.

Chairs record the justification for a document being in scope for the charter at the time of working group adoption on the mailing list.

All consensus decisions are conducted on the mailing list.

# Deliverables

The RPP WG will work on the following milestones within the scope of the charter:

* core architecture, including extension mechanisms (proposed standard)
* specification(s) regarding the provisioning of domain names using RPP (proposed standard)
* mappings between RPP and EPP (proposed standard)
