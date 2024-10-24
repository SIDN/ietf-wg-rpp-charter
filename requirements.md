# Requirements

This is a non-exhaustive list of requirements for the RESTful Provisioning Protocol (RPP)
These requirements will be moved to the working group wiki when it becomes available.

## Authentication

- Support for scalable modern authentication standards (OAuth)
- Fine-granular authorisation model for changes, using framework such as OAuth, beyond current auth-code based authorisation for transfers only

## EPP Compatibility

- Compatible with the existing EPP data model to allow automatic mapping/conversion (possibly in both directions)

## Internationalization

- The contact model must have support for internationalization 
- Email?
- IDNs?

## Extensibilty

- Allow for flexibility in extending data models (for example adding new attributes)

## Data Model

- Commonly used EPP extension may be added to the RPP core data model (example: DNSSEC)

## Expanded features

- Allow for common bulk/listing/filter capabilities

## Architecture

- service discovery - allow for less coupling between clients and servers (HATEOAS)

## Documentation

- OpenAPI as part of the specification would be nice to have

## Extensions

- lightweight process of publishing extensions and implementer-friendly description requirements (like OpenAPI requirement together with extension specification)

## Other

The items below have been mentioned on the lost and may need to be added as an requirement.

- Data Omission - what requirements will there be around a registrar's ability to signal that it has collected some data but has not transmitted it to the registry?  
- Registration attribution - will there be requirements for attribution of registration actions (who did what), and will cryptography be used?  
- Registrant verification - will there be requirements to support registrant verification (NIS2)?  
- Linking - will the protocol support linking to RDAP objects, other RPP objects, etc...  
- Include identification of legal vs. natural contacts.
- Expanded common models (when compared to EPP), maybe there should be much more attributes then it is in EPP (Vatnumber / Company Number/ properties for Identity papers) Trademark information and more There are a lot of epp extensions in the wild that try to handle this.
- include also DNS provisioning as potential use-case
- possibility to seamlessly compose the API with other registry use-cases to have uniform API layer from the client perspective
- investigate possible multi-party authorisation schemas. Use case: DNS operator would get authorisation to update DS or NS record through RPP.
- possibility of mobile app or direct browser integration (use case for registries which directly authenticate their domain holders and allow operations on a domain and/or if RPP would be exposed by a registrar)

