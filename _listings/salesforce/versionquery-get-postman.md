{
  "info": {
    "name": "SalesForce Get Version Query",
    "_postman_id": "c95d0e9a-54d9-4bbb-aae0-bee46a4889af",
    "description": "Executes the specified SOQL query. If the initial query returns only part of the results, the end of the response will contain a field called nextRecordsUrl. In such cases, use the resource {version}/query/{id} to request the next batch of records and repeat until all records have been retrieved.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "c871adac-957a-4a07-92b5-ccd21397bb42",
          "name": "version.get",
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
                  "value": "version",
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
              "id": "b4c17dab-93d5-4251-a55f-1716aa68f807"
            }
          ]
        },
        {
          "id": "fcdb82e8-d303-4c54-b74f-b19a4436f7a1",
          "name": "version.sobjects.get",
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
                  "value": "version",
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
              "id": "6897e0d6-f291-4acb-943f-ea86a0930a6a"
            }
          ]
        },
        {
          "id": "999078d1-2218-463e-a1e1-64b5753ca63b",
          "name": "version.sobjects.sobject.get",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "sobject",
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
              "id": "5c2c6676-dc90-4878-8e01-af6f464dd246"
            }
          ]
        },
        {
          "id": "7a667ec2-0d42-40c5-bdff-d196e2897d1a",
          "name": "version.sobjects.sobject.post",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "sobject",
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
              "id": "b7cf1584-1e4b-44da-9e21-1feb6900f71f"
            }
          ]
        },
        {
          "id": "26dc95c0-f89e-4366-89e9-5bbf7f10224a",
          "name": "version.sobjects.sobject.describe.get",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "sobject",
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
              "id": "a381c670-3163-42db-9d38-e074af472f9b"
            }
          ]
        },
        {
          "id": "e8562edb-ad4e-48ee-975a-fae39ac48fa2",
          "name": "version.sobjects.sobject.id.get",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "sobject",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
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
              "id": "f26c884b-24a0-4528-bb0b-2280e6ef0b02"
            }
          ]
        },
        {
          "id": "0d4f0ae4-ad2f-4ab4-911b-85e68d6054bb",
          "name": "version.sobjects.sobject.id.delete",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "sobject",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
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
              "id": "cf075247-c196-4b81-a86a-6bfb996c1a6c"
            }
          ]
        },
        {
          "id": "c371ac5c-1a78-4979-8fbe-82b076031b9a",
          "name": "version.sobjects.sobject.id.blobField.get",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "sobject",
                  "value": "sobject",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "blobField",
                  "value": "blobField",
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
              "id": "734eb3df-297a-478d-bc99-3a905fc0876b"
            }
          ]
        },
        {
          "id": "dc550316-0551-4668-87f5-f9ddc4ec40c8",
          "name": "version.sobjects.User.id.password.get",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
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
              "id": "1f3409b9-5ba5-4f8c-b63a-7ffdec1bbd28"
            }
          ]
        },
        {
          "id": "c7a02136-ab02-48e7-972f-2d239a38ba00",
          "name": "version.sobjects.User.id.password.post",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
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
              "id": "01eeb9f6-628e-4d06-9f5b-c44292fdcb72"
            }
          ]
        },
        {
          "id": "4625ecc8-b4c8-4a7c-a759-c68d06189c11",
          "name": "version.sobjects.User.id.password.delete",
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
                  "id": "version",
                  "value": "version",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
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
              "id": "73adf17d-823e-48e9-84ab-6620b327450c"
            }
          ]
        },
        {
          "id": "c6072580-5fb3-4774-94dd-a0c6c1f92a6c",
          "name": "version.query.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/query"
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "version",
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
              "id": "77e51fc9-0357-4cf5-84ab-3caac7a36503"
            }
          ]
        }
      ]
    }
  ]
}