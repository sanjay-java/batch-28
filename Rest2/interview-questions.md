#### What do you know about RESTful Web Services?
  - REST stands for Representational State Transfer. REST is defined as the stateless client-server architectural style for developing applications accessed over the web.
  - When web services use HTTP methods to implement the concept of REST architecture, then it is known as RESTful Web services. In this architectural style, data and functionality are served as resources and are accessed by URI (Uniform Resource Identifiers).

#### Explain the advantages of RESTful web services?
  - Enlisted below are the advantages of RESTful web services:
    They are considered as language and platform-independent as these can be written in any programming language and can be executed on any platform. REST is a lightweight protocol and is considered as fast because of less consumption of bandwidth and resources.  It supports multiple technologies and different data formats like plain text, XML, JSON, etc. It has loosely coupled implementation and can be tested easily over browsers.

#### Differentiate SOAP and REST?

#### Explain different HTTP methods supported by RESTful web services?

  - Enlisted below are some common HTTP methods along with their functions that are supported by RESTful web services
    GET: Read-only access to the resource.
    PUT: Creation of new resources.
    DELETE: Removal of a resource.
    POST: Update of an existing resource.
    OPTIONS: Get supported operations on the resource.
    HEAD: Returns HTTP header only, nobody.

#### What is a resource in RESTful web service and how it is represented?

- Resource is said to be a fundamental concept having a type and relationship with other resources. In REST architecture, each content is considered as the resource and they are identified by their URIs. Resources are represented with the help of XML, JSON, text, etc in RESTful architecture.

#### What are the core components of the HTTP request and HTTP response?

  HTTP request has following 5 major components:

  - Verb:	Indicate HTTP methods like GET, PUT, POST, etc
  - URI:	Identifies the resource on server
  - HTTP: Version	Indicates version.
  - Request Header	Contains metadata like client type, cache settings, message body format, etc for HTTP request message.
  - Request Body	Represents content of the message.

  HTTP response has following 4 major components:

  - Status/Response code	Indicates the status of the server for requested resource.
  - HTTP version	Represents HTTP version.
  - Response Header	Consists of metadata like content length, content type, server length, etc for HTTP response message.
  - Response Body	Represents response message content.

#### What is the purpose and format of URI in REST architecture?

  - The purpose of URI is to locate resources on the server that are hosting web services.
    Format of URI:
    <protocol>://<service-name>/<ResourceType>/<ResourceID>  

#### Define SOAP web services?

  - Simple Object Access Protocol (SOAP) is defined as the XML based protocol which is known for designing and developing web services as well as enabling communication between applications developed on different platforms with different programming languages over the Internet. It is both platform and language independent.

#### What are the various approaches available for developing SOAP-based web services?

  - There are basically 2 different approaches available for developing SOAP-based web services. These are explained as follows

  Contract-first approach: In this approach, the contract is defined first by XML and WSDL and then java classes are derived from the contract.
  Contract-last approach: In this approach, java classes are defined first and then the contract is generated which is usually the WSDL file from the java class.
  “Contract-first” method is the most preferred approach.

#### Explain the major obstacle faced by SOAP users?

- One of the major hindrances observed by users of SOAP is the ‘Firewall security mechanism’. In this case, all the HTTP ports except those which bypass firewall is locked. In some cases, a technical issue of mixing specification of message transport with message structure is also observed.

#### What are the advantages and disadvantages of SOAP?

  - Enlisted below are advantages of SOAP web services:

  SOAP allows communications between various applications and it is both language and platform-independent.
  It is very simple as well as uses standard HTTP protocol and XML for sending and receiving messages.
  It defines and uses its own security known as WS security.
  It decouples the encoding and communication protocol from the runtime environment.
  It eradicates firewall problems and is vendor-neutral.
  It allows the circulation of messages in a distributed and decentralized environment.
  Enlisted below are disadvantages of SOAP web services:

  Lightweight formats other than XML are not supported.
  Not easily testable on browsers.
  Security facilities are not present.
  SOAP is slow and cannot be easily tested on the browser.
  Web services and clients are tightly coupled and define some standards that are to be strictly followed.

#### What are the elements of a SOAP message?
  - SOAP is just like other XML document and has the following elements:

  - Envelope: This element is defined as the mandatory root element. It translates the XML document and determines the start and end of the SOAP message.

  - Header: This element contains the optional header attributes of the message that contains specific information on the application. This element can occur multiple times and are intended to add new features and functionalities.
  - Body: This element is mandatory and contains the call and response messages. It is also defined as the child element of the envelope containing all the application derived XML data that has been exchanged as a part of the SOAP message.
  - Fault element: Errors that occur during the processing of the messages are handled by the fault element. If the error is present, then this element appears as a child element of the body. However, there can only be one fault block.

#### What are the important characteristics of the SOAP envelope element?

  - We have seen the basic work of a SOAP envelope element in the previous answer, now let us see some of its characteristics:

  SOAP envelope is a packaging mechanism.
  Every SOAP message has a mandatory root envelope message.
  Only one body element is allowed for each envelope element.
  As the SOAP version changes, envelope changes.
  If the header element is present, it should appear as the first child.
  Prefix ENV and envelope element is used for specification.
  A namespace and an optional encoding style are used in case of optional SOAP encoding.

#### Enlist a few syntax rules applicable for SOAP message?

  - Enlisted below are some important syntax rules that are applicable for SOAP message:

  A SOAP message

  Must be encoded using XML.
  Must use the SOAP envelope namespace.
  Must use the SOAP encoding namespace.
  Must not contain the DTD reference.
  Must not contain XML processing instructions.
