---
name: IBM Watson
x-slug: ibm-watson
description: Meet IBM Watson, a cognitive system that enables a new partnership between
  people and computers that enhances and scales human expertise. Watson has been learning
  the language of professions and is trained by experts to work across many different
  industries.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Internet of Things
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/apis.md
specificationVersion: "0.14"
apis:
- name: IBM Watson IoT Platform HTTP REST API - Query active schema definitions
  x-api-slug: schemas-get
  description: "Schemas are used to define the structure of Events, Device State and\nThing
    State in the Watson IoT Platform.\n\n  - For Events, they define the structure
    of the payload of the events\n    that are published to the platform by devices.\n\n
    \ - For Device and Thing State, they define the structure of the state\n    that
    is stored by the platform.\n\nThe **schemas** endpoint returns the list of all
    of the active schema \ndefinitions for the organization in the Watson IoT Platform.
    \ Various\nquery parameters can be used to filter, sort and page through the list\nof
    schemas that are returned."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/schemas-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/schemas-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get active schema definition metadata
  x-api-slug: schemasschemaid-get
  description: |-
    Retrieves the metadata for the active schema definition with the
    specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/schemasschemaid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/schemasschemaid-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get the contents of the active schema
    definition file
  x-api-slug: schemasschemaidcontent-get
  description: |-
    Retrieves the content of the active schema definition file with the
    specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/schemasschemaidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/schemasschemaidcontent-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Query draft schema definitions
  x-api-slug: draftschemas-get
  description: "Schemas are used to define the structure of Events, Device State and\nThing
    State in the Watson IoT Platform.\n\n  - For Events, they define the structure
    of the payload of the events\n    that are published to the platform by devices.\n\n
    \ - For Device and Thing State, they define the structure of the state\n    that
    is stored by the platform.\n\nThe **/draft/schemas** endpoint returns the list
    of all of the draft \nschema for the organization in the Watson IoT Platform.
    \ Various query\nparameters can be used to filter, sort and page through the list
    of\nschemas that are returned."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftschemas-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftschemas-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Create a draft schema definition
  x-api-slug: draftschemas-post
  description: "Creates a new draft schema definition for the organization in the
    Watson\nIoT Platform.\n\nThe schema definition file is passed to the Watson IoT
    Platform within a\nmultipart POST (multipart/form-data).  The body of the POST
    **must**\ncontain at least two parts:\n\n  - One with a name of **schemaFile**
    that contains the actual content\n    of the file as the body of the part.\n    \n
    \ - One with a name of **name** that contains a string that defines the\n    name
    of the schema resource in the body of the part.\n\nAdditional metadata can be
    passed in other parts within the multipart\nPOST.  For example, to specify a description
    for the new schema\ndefinition, you should include a part with the name **description**
    and\nthe description as the body of the part.  To specify the type of the\nschema,
    you should include a part with the name **schemaType** and one\nof the following
    in the body of the part (the schemaType defaults to\njson-schema if the no schemaType
    part is present):\n\n  - json-schema\n\nIf parts with names other than those specified
    above are included in the\nmultipart POST the request will fail and an HTTP status
    code of 400 will\nbe returned.\n\nThe content of the schema definition file that
    is passed to the platform\nis stored and a REST resource is created containing
    metadata that\ndescribes the schema definition."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftschemas-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftschemas-post-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get draft schema definition metadata
  x-api-slug: draftschemasschemaid-get
  description: |-
    Retrieves the metadata for the draft schema definition with the
    specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftschemasschemaid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftschemasschemaid-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Query active phyiscal interfaces
  x-api-slug: physicalinterfaces-get
  description: |-
    Physical interfaces are used to model the interfaces between physical
    devices and the Watson IoT Platform.  A physical interface references
    event types.  Devices that implement a physical interface publish these
    events to the platform.

    The event types are referenced via a mapping that maps an event id to
    the id of an event type.  The event id corresponds to the MQTT topic
    that the event is published to by a device.

    The **physicalinterfaces** endpoint returns the list of all of the
    active physical interfaces that have been defined for the organization
    in the Watson IoT Platform.  Various query parameters can be used to
    filter, sort and page through the list of active physical interfaces
    that are returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/physicalinterfaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/physicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get an active physical interface
  x-api-slug: physicalinterfacesphysicalinterfaceid-get
  description: Retrieve the active physical interface with the specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceid-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get the list of event mappings
  x-api-slug: physicalinterfacesphysicalinterfaceidevents-get
  description: |-
    Retrieve the list of event mappings for the active physical interface.
    Event mappings are keyed off of the event id specified in the MQTT topic
    that the inbound events are published to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceidevents-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Query draft phyiscal interfaces
  x-api-slug: draftphysicalinterfaces-get
  description: "Physical interfaces are used to model the interfaces between physical\ndevices
    and the Watson IoT Platform.  A physical interface references\nevent types.  Devices
    that implement a physical interface publish these\nevents to the platform.\n\nThe
    event types are referenced via a mapping that maps an event id to\nthe id of an
    event type.  The event id corresponds to the MQTT topic\nthat the event is published
    to by a device.\n\nThe **/draft/physicalinterfaces** endpoint returns the list
    of all of \nthe draft physical interfaces that have been defined for the\norganization
    in the Watson IoT Platform.  Various query parameters can\nbe used to filter,
    sort and page through the list of draft physical\ninterfaces that are returned."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftphysicalinterfaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftphysicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get the list of active property mappings
    for the device type
  x-api-slug: devicetypestypeidmappings-get
  description: |-
    Retrieve the list of active property mappings for the specified device
    type.  A property mapping defines how properties from inbound events are
    mapped to properties defined on an logical interface associated with
    the device type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/devicetypestypeidmappings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/devicetypestypeidmappings-get-openapi.md
- name: |-
    IBM Watson IoT Platform HTTP REST API - Get the active property mappings for a specific logical interface
    for a device type.
  x-api-slug: devicetypestypeidmappingslogicalinterfaceid-get
  description: |-
    Retrieves the active property mappings for a specific logical
    interface for the device type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/devicetypestypeidmappingslogicalinterfaceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/devicetypestypeidmappingslogicalinterfaceid-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get the list of draft property mappings
    for the device type
  x-api-slug: draftdevicetypestypeidmappings-get
  description: |-
    Retrieve the list of draft property mappings for the specified device
    type.  A property mapping defines how properties from inbound events are
    mapped to properties defined on an logical interface associated with
    the device type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftdevicetypestypeidmappings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/draftdevicetypestypeidmappings-get-openapi.md
- name: IBM Watson IoT Platform HTTP REST API - Get the state for the device with
    the specified id
  x-api-slug: devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-get
  description: Retrieve the current state of the device with the specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Machine Learning, Machine Learning, AI, API LIfeyclessss, Stack Network, Stack,
    Getting Started Example, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/internet-of-things/master/_listings/ibm-watson/devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://ibm.financial.crimes.insight.for.insurance.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ibm.watson.stack.network
- type: x-application-gallery
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/gallery.html
- type: x-blog
  url: https://developer.ibm.com/watson/blog/
- type: x-blog-rss
  url: https://developer.ibm.com/watson/feed/
- type: x-developer
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/
- type: x-developer
  url: https://developer.ibm.com/watson/
- type: x-documentation
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/apis/
- type: x-forum
  url: https://developer.ibm.com/answers/smartspace/watson/
- type: x-getting-started
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/getstarted.html
- type: x-github
  url: https://github.com/IBM-Watson
- type: x-partners
  url: http://www.ibm.com/smarterplanet/us/en/ibmwatson/ecosystem.html
- type: x-privacy
  url: http://www.ibm.com/privacy/us/en/?lnk=flg-priv-usen
- type: x-terms-of-service
  url: http://www.ibm.com/legal/us/en/?lnk=flg-tous-usen
- type: x-twitter
  url: https://twitter.com/IBMWatson
- type: x-videos
  url: http://www.ibm.com/smarterplanet/us/en/ibmwatson/
- type: x-website
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
- type: x-white-papers
  url: https://developer.ibm.com/watson/docs/whitepapers/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---