---
swagger: "2.0"
x-collection-name: Salesforce
x-complete: 0
info:
  title: SalesForce Delete Version Sobjects User  Password
  description: Resets an user password. Salesforce will reset the user password to
    an auto-generated password, which will be returned in the response.
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}:
    get:
      summary: Get Version
      description: Lists available resources for the specified API version, including
        resource name and URI.
      operationId: version.get
      x-api-path-slug: version-get
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
      operationId: version.sobjects.get
      x-api-path-slug: versionsobjects-get
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
      operationId: version.sobjects.sobject.get
      x-api-path-slug: versionsobjectssobject-get
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - Sobject
    post:
      summary: Add Version Sobjects Sobject
      description: Creates a new object.
      operationId: version.sobjects.sobject.post
      x-api-path-slug: versionsobjectssobject-post
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
      operationId: version.sobjects.sobject.describe.get
      x-api-path-slug: versionsobjectssobjectdescribe-get
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
      operationId: version.sobjects.sobject.id.get
      x-api-path-slug: versionsobjectssobjectid-get
      parameters:
      - in: query
        name: fields
        description: Optional list of fields used to return values for
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
      operationId: version.sobjects.sobject.id.delete
      x-api-path-slug: versionsobjectssobjectid-delete
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - Sobject
  /{version}/sobjects/{sobject}/{id}/{blobField}:
    get:
      summary: Get Version Sobjects Sobject  Blobfield
      description: Retrieves the specified blob field from an individual record. Because
        blob fields contain binary data, you can't use JSON or XML to retrieve this
        data.
      operationId: version.sobjects.sobject.id.blobField.get
      x-api-path-slug: versionsobjectssobjectidblobfield-get
      parameters:
      - in: query
        name: fields
        description: Optional list of fields used to return values for
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - Sobject
      - ""
      - Blobfield
  /{version}/sobjects/User/{id}/password:
    get:
      summary: Get Version Sobjects User  Password
      description: Gets password expiration status for a given user. The session must
        have permission to access the given user password information, otherwise an
        error response is returned.
      operationId: version.sobjects.User.id.password.get
      x-api-path-slug: versionsobjectsuseridpassword-get
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - User
      - ""
      - Password
    post:
      summary: Add Version Sobjects User  Password
      description: Changes the password for a given user ID. The new password must
        conform to the password policies for the organization, otherwise you will
        get an error response. You can only change one password per request.
      operationId: version.sobjects.User.id.password.post
      x-api-path-slug: versionsobjectsuseridpassword-post
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - User
      - ""
      - Password
    delete:
      summary: Delete Version Sobjects User  Password
      description: Resets an user password. Salesforce will reset the user password
        to an auto-generated password, which will be returned in the response.
      operationId: version.sobjects.User.id.password.delete
      x-api-path-slug: versionsobjectsuseridpassword-delete
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - User
      - ""
      - Password
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