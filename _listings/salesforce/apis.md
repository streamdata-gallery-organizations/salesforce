---
name: Salesforce
x-slug: salesforce
description: Build more meaningful and lasting relationships and connect with your
  customers across sales, customer service, marketing, communities, apps, analytics,
  and more using our Customer Success Platform. Try for Free.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
x-kinRank: "10"
x-alexaRank: "146"
tags: Salesforce
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/apis.md
specificationVersion: "0.14"
apis:
- name: SalesForce Get Version
  x-api-slug: salesforce
  description: Lists available resources for the specified API version, including
    resource name and URI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}
  tags: Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/version-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/version-get-openapi.md
- name: SalesForce Get Version Sobjects
  x-api-slug: salesforce
  description: Lists the available objects and their metadata for your organization's
    data. In addition, it provides the organization encoding, as well as maximum batch
    size permitted in queries. For more information, see Internationalization and
    Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects
  tags: Version, Sobjects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjects-get-openapi.md
- name: SalesForce Get Version Sobjects Sobject
  x-api-slug: salesforce
  description: Retrieves the metadata for an object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobject-get-openapi.md
- name: SalesForce Add Version Sobjects Sobject
  x-api-slug: salesforce
  description: Creates a new object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobject-post-openapi.md
- name: SalesForce Get Version Sobjects Sobject Describe
  x-api-slug: salesforce
  description: Completely describes the individual metadata at all levels for the
    specified object. For example, this can be used to retrieve the fields, URLs,
    and child relationships for the Account object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/describe
  tags: Version, Sobjects, Sobject, Describe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectdescribe-get-openapi.md
- name: SalesForce Get Version Sobjects Sobject
  x-api-slug: salesforce
  description: Retrieves individual records for an object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/{id}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectid-get-openapi.md
- name: SalesForce Delete Version Sobjects Sobject
  x-api-slug: salesforce
  description: Deletes a record.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/{id}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectid-delete-openapi.md
- name: SalesForce Get Version Sobjects Sobject  Blobfield
  x-api-slug: salesforce
  description: Retrieves the specified blob field from an individual record. Because
    blob fields contain binary data, you can't use JSON or XML to retrieve this data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/{id}/{blobField}
  tags: Version, Sobjects, Sobject, , Blobfield
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectidblobfield-get-openapi.md
- name: SalesForce Get Version Sobjects User  Password
  x-api-slug: salesforce
  description: Gets password expiration status for a given user. The session must
    have permission to access the given user password information, otherwise an error
    response is returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/User/{id}/password
  tags: Version, Sobjects, User, , Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-get-openapi.md
- name: SalesForce Add Version Sobjects User  Password
  x-api-slug: salesforce
  description: Changes the password for a given user ID. The new password must conform
    to the password policies for the organization, otherwise you will get an error
    response. You can only change one password per request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/User/{id}/password
  tags: Version, Sobjects, User, , Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-post-openapi.md
- name: SalesForce Delete Version Sobjects User  Password
  x-api-slug: salesforce
  description: Resets an user password. Salesforce will reset the user password to
    an auto-generated password, which will be returned in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/User/{id}/password
  tags: Version, Sobjects, User, , Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-delete-openapi.md
- name: SalesForce Get Version Query
  x-api-slug: salesforce
  description: Executes the specified SOQL query. If the initial query returns only
    part of the results, the end of the response will contain a field called nextRecordsUrl.
    In such cases, use the resource {version}/query/{id} to request the next batch
    of records and repeat until all records have been retrieved.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/query
  tags: Version, Query
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionquery-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionquery-get-openapi.md
- name: SalesForce Get Version Query
  x-api-slug: salesforce
  description: 'Retrieves the remaining SOQL query results using the identifier within
    the field "nextRecordsUrl" value (i.e. "nextRecordsUrl" : "/services/data/v24.0/query/01gD0000002HU6KIAW-2000")
    located at the end of the initial query results. Requests the next batch of records
    and you could repeat (using the corresponding identifier) until all records have
    been retrieved.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/query/{id}
  tags: Version, Query
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionqueryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionqueryid-get-openapi.md
- name: SalesForce Get Version Search
  x-api-slug: salesforce
  description: Executes the specified SOSL search. The search string must be URL-encoded.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data//{version}/search
  tags: Version, Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsearch-get-openapi.md
- name: SalesForce
  x-api-slug: salesforce
  description: Build more meaningful and lasting relationships and connect with your
    customers across sales, customer service, marketing, communities, apps, analytics,
    and more using our Customer Success Platform. Try for Free.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data
  tags: Salesforce
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/openapi.md
- name: Salesforce Sandbox Get
  x-api-slug: salesforce-sandbox
  description: Lists summary information about each Salesforce version currently available,
    including the version, label, and a link to each version's root.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///
  tags: ""
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/get-openapi.md
- name: Salesforce Sandbox Get Version
  x-api-slug: salesforce-sandbox
  description: Lists available resources for the specified API version, including
    resource name and URI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}
  tags: Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/version-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/version-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects
  x-api-slug: salesforce-sandbox
  description: Lists the available objects and their metadata for your organization's
    data. In addition, it provides the organization encoding, as well as maximum batch
    size permitted in queries. For more information, see Internationalization and
    Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects
  tags: Version,Sobjects
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjects-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjects-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Retrieves the metadata for an object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobject-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobject-get-openapi.md
- name: Salesforce Sandbox Post Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Creates a new object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobject-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobject-post-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject Describe
  x-api-slug: salesforce-sandbox
  description: Completely describes the individual metadata at all levels for the
    specified object. For example, this can be used to retrieve the fields, URLs,
    and child relationships for the Account object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/describe
  tags: Version,Sobjects,Sobject,Describe
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectdescribe-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectdescribe-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Retrieves individual records for an object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/{id}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectid-get-openapi.md
- name: Salesforce Sandbox Delete Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Deletes a record.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/{id}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectid-delete-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject Blobfield
  x-api-slug: salesforce-sandbox
  description: Retrieves the specified blob field from an individual record. Because
    blob fields contain binary data, you can't use JSON or XML to retrieve this data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/{id}/{blobField}
  tags: Version,Sobjects,Sobject,Blobfield
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectidblobfield-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectssobjectidblobfield-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects User Password
  x-api-slug: salesforce-sandbox
  description: Gets password expiration status for a given user. The session must
    have permission to access the given user password information, otherwise an error
    response is returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/User/{id}/password
  tags: Version,Sobjects,User,Password
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-get-openapi.md
- name: Salesforce Sandbox Post Version Sobjects User Password
  x-api-slug: salesforce-sandbox
  description: Changes the password for a given user ID. The new password must conform
    to the password policies for the organization, otherwise you will get an error
    response. You can only change one password per request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/User/{id}/password
  tags: Version,Sobjects,User,Password
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-post-openapi.md
- name: Salesforce Sandbox Delete Version Sobjects User Password
  x-api-slug: salesforce-sandbox
  description: Resets an user password. Salesforce will reset the user password to
    an auto-generated password, which will be returned in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/User/{id}/password
  tags: Version,Sobjects,User,Password
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsobjectsuseridpassword-delete-openapi.md
- name: Salesforce Sandbox Get Version Query
  x-api-slug: salesforce-sandbox
  description: Executes the specified SOQL query. If the initial query returns only
    part of the results, the end of the response will contain a field called nextRecordsUrl.
    In such cases, use the resource {version}/query/{id} to request the next batch
    of records and repeat until all records have been retrieved.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/query
  tags: Version,Query
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionquery-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionquery-get-openapi.md
- name: Salesforce Sandbox Get Version Query
  x-api-slug: salesforce-sandbox
  description: 'Retrieves the remaining SOQL query results using the identifier within
    the field "nextRecordsUrl" value (i.e. "nextRecordsUrl" : "/services/data/v24.0/query/01gD0000002HU6KIAW-2000")
    located at the end of the initial query results. Requests the next batch of records
    and you could repeat (using the corresponding identifier) until all records have
    been retrieved.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/query/{id}
  tags: Version,Query
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionqueryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionqueryid-get-openapi.md
- name: Salesforce Sandbox Get Version Search
  x-api-slug: salesforce-sandbox
  description: Executes the specified SOSL search. The search string must be URL-encoded.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data///{version}/search
  tags: Version,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/versionsearch-get-openapi.md
- name: Salesforce Sandbox
  x-api-slug: salesforce-sandbox
  description: Build more meaningful and lasting relationships and connect with your
    customers across sales, customer service, marketing, communities, apps, analytics,
    and more using our Customer Success Platform. Try for Free.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/175-salesforce.jpg
  humanURL: http://salesforce.com
  baseURL: https://na14.salesforce.com//services/data/
  tags: Salesforce
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesforce/master/_listings/salesforce/openapi.md
x-common:
- type: x-base
  url: https://na1.salesforce.com
- type: x-blog
  url: https://developer.salesforce.com/blogs/
- type: x-blog-rss
  url: http://feeds.feedburner.com/SforceBlog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/salesforce
- type: x-crunchbase
  url: https://crunchbase.com/organization/salesforce
- type: x-email
  url: legal@salesforce.com
- type: x-email
  url: copyright@salesforce.com
- type: x-email
  url: legalcompliance@salesforce.com
- type: x-email
  url: trademarks@salesforce.com
- type: x-email
  url: privacymark@salesforce.com
- type: x-email
  url: marketingcloudsupport@salesforce.com
- type: x-email
  url: support@desk.com
- type: x-email
  url: credits@salesforce.com
- type: x-email
  url: privacy@salesforce.com
- type: x-github
  url: https://github.com/salesforce
- type: x-partners
  url: https://partners.salesforce.com/
- type: x-twitter
  url: https://twitter.com/salesforcedevs
- type: x-twitter
  url: https://twitter.com/salesforce
- type: x-website
  url: http://salesforce.com
- type: x-website
  url: https://developer.salesforce.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---