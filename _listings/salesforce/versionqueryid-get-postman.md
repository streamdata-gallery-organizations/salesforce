{
  "info": {
    "name": "Salesforce Sandbox Get Version Query",
    "_postman_id": "f8dbde80-ec99-47e8-abb3-91585907d69c",
    "description": "Retrieves the remaining SOQL query results using the identifier within the field \"nextRecordsUrl\" value (i.e. \"nextRecordsUrl\" : \"/services/data/v24.0/query/01gD0000002HU6KIAW-2000\") located at the end of the initial query results. Requests the next batch of records and you could repeat (using the corresponding identifier) until all records have been retrieved.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "cb20f197-81c4-4bde-97a9-7ac1c0a8b890",
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
              "id": "6cb49d91-6838-4bd1-8a7c-1873682628e7"
            }
          ]
        }
      ]
    },
    {
      "name": "Version",
      "item": [
        {
          "id": "586a7f21-09ff-484b-b203-93364cc526aa",
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
              "id": "f16d62ba-7809-40c7-9778-58ddb7ab2888"
            }
          ]
        },
        {
          "id": "e0395e15-1555-4929-8e06-61f86ac1f766",
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
              "id": "2e431437-16f2-4a3a-9d5b-f3aa421c9950"
            }
          ]
        },
        {
          "id": "565c4e38-e242-42b9-9cce-f4092bfc2fb3",
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
              "id": "c6a76903-8e74-4ad5-8ede-15e9df37daa9"
            }
          ]
        },
        {
          "id": "409e1ba6-3fdd-48ce-bd9a-325b50b3f6a7",
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
              "id": "4cb33fff-ce2b-455d-b181-6635e32dd8a7"
            }
          ]
        },
        {
          "id": "30e0d01d-448b-4201-9a75-6f67565f5c48",
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
              "id": "1103b804-570f-47c8-aab0-aaef1aa94c53"
            }
          ]
        },
        {
          "id": "8f2432be-7b95-4e32-93ba-5c96aa6c83b1",
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
              "id": "0b0b8c31-35f8-4e0c-b1ff-3e6878adfbfd"
            }
          ]
        },
        {
          "id": "24eda733-8c88-4d9d-ad76-afd69fe5edf4",
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
              "id": "3e709738-17f2-4438-8d4d-3ec8f5f5fc9e"
            }
          ]
        },
        {
          "id": "6bf00795-be1a-4904-adf3-f65c41ff6356",
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
              "id": "d14e41f1-d6eb-4a75-bd54-d8499711df9b"
            }
          ]
        },
        {
          "id": "085de3f4-1dc8-4ea5-a3e3-a18d91b570a5",
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
              "id": "ac9b90ce-582c-425f-9f67-e64bc45e735a"
            }
          ]
        },
        {
          "id": "2f45bc3a-6215-4b28-a19c-23e46cb4e71b",
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
              "id": "e6fca020-9c6c-462b-9f46-14112ba9d5b3"
            }
          ]
        },
        {
          "id": "5b9d01e5-e0ec-416b-b163-740d912f11fe",
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
              "id": "c0b98824-3a5a-4619-ae7f-986a472d43d6"
            }
          ]
        },
        {
          "id": "35a05526-5495-4e57-8755-0eadc95862d8",
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
              "id": "54e06ccc-0d40-4b29-9588-0f01daf43369"
            }
          ]
        },
        {
          "id": "af67250c-bd9f-46c9-acaf-329b826cd3b1",
          "name": "getVersionQuery",
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
            "description": "Retrieves the remaining SOQL query results using the identifier within the field \"nextRecordsUrl\" value (i.e. \"nextRecordsUrl\" : \"/services/data/v24.0/query/01gD0000002HU6KIAW-2000\") located at the end of the initial query results. Requests the next batch of records and you could repeat (using the corresponding identifier) until all records have been retrieved."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2fd45e9-13dc-46c8-b56b-dc576fb31f7c"
            }
          ]
        }
      ]
    }
  ]
}