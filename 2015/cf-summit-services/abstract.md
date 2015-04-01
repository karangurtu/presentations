# CF Service Brokers Updates: Async provisions, service keys, and any params

## Abstract

CloudFoundry Services make up the most extensible part of any CF installation. The architecture is flexible and uses a broker model allows for various types of services to be integrated and used in any CF installations.

While very powerful and flexible, the current CF Services architecture had some major pending issues that prevented CF installations to be even more useful and capable. In particular, using the current architecture, it was difficult to integrate analytics types of services, as well as allowing service instances to be used outside of CF applications.

Recent enhancements to the CF services architecture attempt to address the current limitations by adding three key new features. First, services can now be provisioned and de-provisioned in an async fashion which allows service brokers to take whatever amount of time needed to create and delete their managed service instances.

Second, service brokers can now issue keys (credentials) to any client without having a need for a CF application. This allows a CF service to be used in a client that lives outside of the CF installation, e.g., a Docker container application. And finally, service brokers can now exchange any number of parameters for their service instances.

In this talk, the newly formed CF Services APIs team will review the Service Broker architecture that CF provides, discuss in details the new features, and show examples (and demos) of how the new features can be used to solve problems in current CF offerings.

