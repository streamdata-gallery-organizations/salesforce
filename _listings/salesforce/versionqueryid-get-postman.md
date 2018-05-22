{
  "info": {
    "name": "SalesForce Get Version Query",
    "_postman_id": "69ef8091-43a8-4a71-86c4-d0d65776df16",
    "description": "Retrieves the remaining SOQL query results using the identifier within the field \"nextRecordsUrl\" value (i.e. \"nextRecordsUrl\" : \"/services/data/v24.0/query/01gD0000002HU6KIAW-2000\") located at the end of the initial query results. Requests the next batch of records and you could repeat (using the corresponding identifier) until all records have been retrieved.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "f8fdd2ef-aace-439c-94f5-ed96eaabb077",
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
              "id": "2cd92f84-731e-49c6-ac70-1e5646aae7db"
            }
          ]
        },
        {
          "id": "533b09fa-24a7-4560-ab5b-734381403dad",
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
              "id": "bb19691b-2f95-4ef6-a0b0-e2bc52881078"
            }
          ]
        },
        {
          "id": "46d3f0b5-4abc-4380-a780-cfd61e4ed5d1",
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
              "id": "48b638c3-88c7-4f6c-9e37-d0fa22ad5e49"
            }
          ]
        },
        {
          "id": "3259c1a5-935d-47f2-af8e-09e7e7ef8f3f",
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
              "id": "742ed461-84f0-4198-a714-d85776a3d191"
            }
          ]
        },
        {
          "id": "54a35f3d-21ad-4c03-bc83-ab2e60a35f63",
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
              "id": "3e00ca74-06fd-4ad4-8999-f8254da130bd"
            }
          ]
        },
        {
          "id": "d52def80-8efd-43ea-a8f1-1a314d210b7f",
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
              "id": "a1620787-a458-410d-9fd8-f5b06476fadd"
            }
          ]
        },
        {
          "id": "42683ac8-9ba0-4889-82dd-2bac826d17bf",
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
              "id": "483f0a74-c79f-4399-992b-5b9f5e959b5e"
            }
          ]
        },
        {
          "id": "433dfd32-e999-451b-b530-77191667c2da",
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
              "id": "253aff65-9d03-45d8-99c4-1b4477102748"
            }
          ]
        },
        {
          "id": "7d00dbac-0cf1-4ae3-885b-2bb85a42475d",
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
              "id": "43996e14-e127-4fda-aaa4-781299a9a3a2"
            }
          ]
        },
        {
          "id": "6aa8341e-9632-4409-8d24-1883eee14ebf",
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
              "id": "92d2afa5-cd53-4a1b-87be-b35d5b1e0639"
            }
          ]
        },
        {
          "id": "758ded4b-8592-4546-9d92-f7a9b1a421fc",
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
              "id": "e6f7b384-9658-432a-9ae9-0bafd2ec9ce1"
            }
          ]
        },
        {
          "id": "184d7fd9-aecc-43c8-a31a-ea3db73b2192",
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
              "id": "50f1eb9d-3463-4b5d-90ed-40f63893ff26"
            }
          ]
        },
        {
          "id": "8d597c57-2ca2-4556-b3e2-0e475f659de0",
          "name": "version.query.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/query/:id"
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
            "description": "Retrieves the remaining SOQL query results using the identifier within the field \"nextRecordsUrl\" value (i.e. \"nextRecordsUrl\" : \"/services/data/v24.0/query/01gD0000002HU6KIAW-2000\") located at the end of the initial query results. Requests the next batch of records and you could repeat (using the corresponding identifier) until all records have been retrieved."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb447d6c-92cb-4290-bbcb-ea3b337ed5bc"
            }
          ]
        }
      ]
    }
  ]
}