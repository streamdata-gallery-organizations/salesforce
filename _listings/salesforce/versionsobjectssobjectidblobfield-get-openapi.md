---
swagger: "2.0"
x-collection-name: Salesforce
x-complete: 0
info:
  title: Salesforce Sandbox Get Version Sobjects Sobject Blobfield
  description: Retrieves the specified blob field from an individual record. Because
    blob fields contain binary data, you can't use JSON or XML to retrieve this data.
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
  /{version}/sobjects/{sobject}/describe:
    get:
      summary: Get Version Sobjects Sobject Describe
      description: Completely describes the individual metadata at all levels for
        the specified object. For example, this can be used to retrieve the fields,
        URLs, and child relationships for the Account object.
      operationId: getVersionSobjectsSobjectDescribe
      x-api-path-slug: versionsobjectssobjectdescribe-get
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
      - Describe
  /{version}/sobjects/{sobject}/{id}:
    get:
      summary: Get Version Sobjects Sobject
      description: Retrieves individual records for an object.
      operationId: getVersionSobjectsSobject
      x-api-path-slug: versionsobjectssobjectid-get
      parameters:
      - in: query
        name: fields
        description: Optional list of fields used to return values for
      - in: path
        name: id
        description: A Salesforces object ID
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
    delete:
      summary: Delete Version Sobjects Sobject
      description: Deletes a record.
      operationId: deleteVersionSobjectsSobject
      x-api-path-slug: versionsobjectssobjectid-delete
      parameters:
      - in: path
        name: id
        description: A Salesforces object ID
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
  /{version}/sobjects/{sobject}/{id}/{blobField}:
    get:
      summary: Get Version Sobjects Sobject Blobfield
      description: Retrieves the specified blob field from an individual record. Because
        blob fields contain binary data, you can't use JSON or XML to retrieve this
        data.
      operationId: getVersionSobjectsSobjectBlobfield
      x-api-path-slug: versionsobjectssobjectidblobfield-get
      parameters:
      - in: path
        name: blobField
        description: A Salesforces object blob field
      - in: query
        name: fields
        description: Optional list of fields used to return values for
      - in: path
        name: id
        description: A Salesforces object ID
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
      - Blobfield
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