{
  "info": {
    "name": "Salesforce Sandbox Get Version Query",
    "_postman_id": "82b57484-7415-4872-bf99-8277b779edee",
    "description": "Executes the specified SOQL query. If the initial query returns only part of the results, the end of the response will contain a field called nextRecordsUrl. In such cases, use the resource {version}/query/{id} to request the next batch of records and repeat until all records have been retrieved.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "b1a6a86a-b2e0-4e6c-ba92-211347d50c92",
          "name": "get",
          "request": {
            "url": "http://na14.salesforce.com/services/data/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists summary information about each Salesforce version currently available, including the version, label, and a link to each version's root."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8282167-57a4-42dd-9f22-0d28cfe7270c"
            }
          ]
        }
      ]
    },
    {
      "name": "Version",
      "item": [
        {
          "id": "56f3114f-838d-48e2-8210-d0a85b4689b2",
          "name": "getVersion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version"
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
            "description": "Lists available resources for the specified API version, including resource name and URI."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90d1b6dc-1ce0-4b70-914e-bc36d78802fb"
            }
          ]
        },
        {
          "id": "304f1fe8-fd34-476a-8342-9ed57bfd9cd9",
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
              "id": "3d1df550-334a-4a28-a50b-e6e16d2002e5"
            }
          ]
        },
        {
          "id": "9df8dd51-dc8a-4112-a165-d1f5bbe04b2b",
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
              "id": "78d0d0c6-e5f9-4e99-bf7f-bf2f28059c20"
            }
          ]
        },
        {
          "id": "af223b96-1c9c-4a44-a96b-e0f7c255a46a",
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
              "id": "cbec7e1a-4b7b-4bab-8dd2-6c9acd643f43"
            }
          ]
        },
        {
          "id": "14e78d06-a5dc-48ed-8ecc-3d1a13358c5f",
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
              "id": "10a8cb0b-a917-428e-8940-1ae581931bab"
            }
          ]
        },
        {
          "id": "0d5e7049-6736-4127-ad7d-34d01e91a1d9",
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
              "id": "b0db9d16-9fa5-41ad-9c7c-9101d9433d67"
            }
          ]
        },
        {
          "id": "26be58a0-e021-4f39-9542-bed744b7ed7b",
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
              "id": "124e4be0-b925-4e0e-9bbe-68e313f9b546"
            }
          ]
        },
        {
          "id": "befd50b6-9c76-4f70-842c-c9206e9f1098",
          "name": "getVersionSobjectsSobjectBlobfield",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/:id/:blobField"
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
                  "id": "blobField",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Retrieves the specified blob field from an individual record. Because blob fields contain binary data, you can't use JSON or XML to retrieve this data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bca2d0b6-47d8-49d5-a5de-c415ee441997"
            }
          ]
        },
        {
          "id": "39f88d16-376d-4f3d-91ea-4e105d3e1151",
          "name": "getVersionSobjectsUserPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/User/:id/password"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Gets password expiration status for a given user. The session must have permission to access the given user password information, otherwise an error response is returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4a36f72-c50d-4555-ab4e-97d828c5f320"
            }
          ]
        },
        {
          "id": "d0201d8b-f5fb-4d06-a1ab-027284bda192",
          "name": "postVersionSobjectsUserPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/User/:id/password"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Changes the password for a given user ID. The new password must conform to the password policies for the organization, otherwise you will get an error response. You can only change one password per request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94ea2d3f-f079-4e00-845c-aee86a003427"
            }
          ]
        },
        {
          "id": "a78841a6-d772-4f76-a839-1f0b4f6c7e44",
          "name": "deleteVersionSobjectsUserPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/User/:id/password"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Resets an user password. Salesforce will reset the user password to an auto-generated password, which will be returned in the response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87813d2d-493f-416f-b12c-be4f833b8d54"
            }
          ]
        },
        {
          "id": "a35141ea-9b8d-4bf6-a925-467cc73b19ea",
          "name": "getVersionQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/query"
              ],
              "query": [
                {
                  "key": "q",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Executes the specified SOQL query. If the initial query returns only part of the results, the end of the response will contain a field called nextRecordsUrl. In such cases, use the resource {version}/query/{id} to request the next batch of records and repeat until all records have been retrieved."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bbc644c-a78f-4aa7-b49b-851cb574ad8f"
            }
          ]
        }
      ]
    }
  ]
}