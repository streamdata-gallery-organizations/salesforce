{
  "info": {
    "name": "Salesforce Sandbox Delete Version Sobjects Sobject",
    "_postman_id": "436a952b-56bc-4164-965e-1aa38346b4cf",
    "description": "Deletes a record.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "947821a6-39e4-4f7c-84a2-f6c77c4c4cba",
          "name": "getVersionSobjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects"
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the available objects and their metadata for your organization's data. In addition, it provides the organization encoding, as well as maximum batch size permitted in queries. For more information, see Internationalization and Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c695dd7-bdf5-4305-91fb-81f228214ed6"
            }
          ]
        },
        {
          "id": "76ad9f48-b540-416c-952d-ed45c9d854ce",
          "name": "getVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject"
              ],
              "variable": [
                {
                  "id": "sobject",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the metadata for an object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee6906e1-470a-4146-8f2a-2d7ff75298a9"
            }
          ]
        },
        {
          "id": "cb17b746-00c6-4e5e-b7f8-2dae813323a2",
          "name": "postVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject"
              ],
              "variable": [
                {
                  "id": "sobject",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "530e2adf-1e5e-4d68-aea8-27f05d8a443c"
            }
          ]
        },
        {
          "id": "c944e372-894f-4b6d-8e8a-1a657e603128",
          "name": "getVersionSobjectsSobjectDescribe",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/describe"
              ],
              "variable": [
                {
                  "id": "sobject",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Completely describes the individual metadata at all levels for the specified object. For example, this can be used to retrieve the fields, URLs, and child relationships for the Account object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72f046c1-352f-4d3b-b9ae-b134e95afc57"
            }
          ]
        },
        {
          "id": "80555d14-ccc1-48db-88c3-c5cab0d3641a",
          "name": "getVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/:id"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves individual records for an object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf3afd84-e546-4061-b9b6-e8d47f5394b1"
            }
          ]
        },
        {
          "id": "4323ff1f-fc1e-4f79-af2e-b6d54f35be56",
          "name": "deleteVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a record."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b3d44c6-c62a-41aa-aadf-1c0e3d7390fc"
            }
          ]
        }
      ]
    }
  ]
}