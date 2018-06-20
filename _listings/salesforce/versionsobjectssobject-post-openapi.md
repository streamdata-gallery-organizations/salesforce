---
swagger: "2.0"
x-collection-name: Salesforce
x-complete: 0
info:
  title: Salesforce Sandbox Post Version Sobjects Sobject
  description: Creates a new object.
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Get
      description: Lists summary information about each Salesforce version currently
        available, including the version, label, and a link to each version's root.
      operationId: get
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - ""
  /{version}:
    get:
      summary: Get Version
      description: Lists available resources for the specified API version, including
        resource name and URI.
      operationId: getVersion
      x-api-path-slug: version-get
      parameters:
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
  /{version}/sobjects:
    get:
      summary: Get Version Sobjects
      description: Lists the available objects and their metadata for your organization's
        data. In addition, it provides the organization encoding, as well as maximum
        batch size permitted in queries. For more information, see Internationalization
        and Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization).
      operationId: getVersionSobjects
      x-api-path-slug: versionsobjects-get
      parameters:
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
  /{version}/sobjects/{sobject}:
    get:
      summary: Get Version Sobjects Sobject
      description: Retrieves the metadata for an object.
      operationId: getVersionSobjectsSobject
      x-api-path-slug: versionsobjectssobject-get
      parameters:
      - in: path
        name: sobject
        description: A Salesforces object
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - Sobject
    post:
      summary: Post Version Sobjects Sobject
      description: Creates a new object.
      operationId: postVersionSobjectsSobject
      x-api-path-slug: versionsobjectssobject-post
      parameters:
      - in: path
        name: sobject
        description: A Salesforces object
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - Sobject
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---