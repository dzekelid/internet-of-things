---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 1
info:
  title: EVRYTHNG
  description: the-evrythng-platform-is-a-cloud-platformasaservice-paas-for-storing-sharing-and-analyzing-data-generated-by-physical-objects--the-platform-gives-a-unique-and-permanent-digital-identity-also-known-as-adis-to-each-individual-object-and-allows-authorized-applications-and-users-to-access-it-via-rest-and-pubsub-mqtt-apis--visualisations-in-the-evrythng-dashboard-analytics-conditional-redirections-and-the-reactor-rules-engine-provide-means-to-add-intelligent-behavior-and-features-on-top-of-your-data-to-add-value-
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /thngs/{THNG_ID}/location:
    put:
      summary: /thngs/{id}/location (U)
      description: USER updates the location of a thng.
      operationId: ThngsLocationByTHNGIDPut
      x-api-path-slug: thngsthng-idlocation-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: THNG_ID
      responses:
        200:
          description: OK
      tags:
      - Thngs
      - THNG
      - ID
      - Location
  /thngs:
    get:
      summary: /thngs (O)
      description: OPERATOR reads the list of all thngs in the account.
      operationId: ThngsGet
      x-api-path-slug: thngs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Thngs
    post:
      summary: /thngs (O)
      description: Creates a thng that is visible by no Applications
      operationId: ThngsPost
      x-api-path-slug: thngs-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Thngs
---