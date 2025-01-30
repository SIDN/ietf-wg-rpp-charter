# Introduction

The Extensible Provisioning Protocol (EPP) was standardized ([STD69](https://datatracker.ietf.org/doc/std69/)) in 2009 to address the needs of domain name management between domain name registries and registrars.
Though EPP is still serving the domain name industry well, the progress in available development, integration and operational patterns, tools and technologies create a desire to have a provisioning protocol using the REST architectural style and the JSON data-interchange format. 
Such design is expected to take advantage of stateless architecture and widely deployed solutions such as OpenAPI, associated documentation, testing and code generation tools, and L4-L7 network services such as API gateways, authorization servers, load balancers, web servers, web application firewalls, etc. 
The successful adoption of Registration Data Access Protocol (RDAP) by Domain Name Registries (DNRs) and Regional Internet Registries (RIRs) demonstrates the usefulness of JSON and REST based architectures.

Production deployments of REST and JSON based provisioning protocols by Country Code Top Level Domains (ccTLDs) have been well received, however variance across implementations is starting to become a concern.

A standardized REST architecture is expected to allow easier integration between registries and registrars, thus lowering the costs for domain registration and new market entrants.

# Scope

The RPP working group is focused on designing a new protocol via a series of specifications known collectively as the RESTful Provisioning Protocol (RPP).

These specifications target at least level 2 of the Richardson Maturity Model, using HTTPS and JSON. 

The RPP WG considers functional equivalents of functionality from EPP for domain names, hosts and contacts ([RFC5730](https://datatracker.ietf.org/doc/html/rfc5730), [5731](https://datatracker.ietf.org/doc/html/rfc5731), [5732](https://datatracker.ietf.org/doc/html/rfc5732), and [5733](https://datatracker.ietf.org/doc/html/rfc5733)) and mappings for data objects, operations, commands and responses.

New functionalities, not having any equivalents in EPP or [EPP extensions](https://www.iana.org/assignments/epp-extensions/epp-extensions.xhtml), may be defined for RPP.

Given that RPP is intended to co-exist alongside EPP, considerations for replacing EPP or migration scenarios away from EPP are outside the scope of the RPP WG.

The REGEXT working group is chartered to maintain and standardize extensions to EPP. 
Consequently, any extensions or changes to EPP, including those related to RPP functionality that do not exist in EPP, are explicitly out of scope for the RPP working group. 

RPP resources are secured with appropriately strong authentication, only encrypted transports are used to properly safeguard authentication material.

Security requirements for RPP are intentionally generic, enabling operators to choose the specific authentication mechanisms and degree of automation that is supported.

# Deliverables

The RPP WG will work on the following milestones within the scope of the charter:

* core architecture, including extension mechanisms (proposed standard)
* specification(s) regarding the provisioning of domain names using RPP (proposed standard)
* mappings between RPP and EPP (proposed standard)
