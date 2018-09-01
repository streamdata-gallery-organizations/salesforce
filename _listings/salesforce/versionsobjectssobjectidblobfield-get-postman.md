{
  "info": {
    "name": "Salesforce Sandbox Get Version Sobjects Sobject Blobfield",
    "_postman_id": "206dbb1c-54d5-43f1-8532-f48f450cbf2a",
    "description": "Retrieves the specified blob field from an individual record. Because blob fields contain binary data, you can't use JSON or XML to retrieve this data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "b279ac0a-c7fd-4503-a72d-8ca7a9f6ac52",
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
              "id": "d23abc7f-edfd-42ad-96d2-64f275f102f9"
            }
          ]
        },
        {
          "id": "e340fc46-8cb1-4472-b4d9-26170d42cff3",
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
              "id": "b83746d1-72a3-469d-b57e-6509412d1d02"
            }
          ]
        },
        {
          "id": "db7c1b13-77fb-4157-a091-d4816113e68e",
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
              "id": "a7fc2fc3-fa1f-476d-b0e8-9d5043dfd668"
            }
          ]
        },
        {
          "id": "f0fd6681-11bc-4925-ba39-2e32618ee27d",
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
              "id": "b1a7f979-6ce2-4f7d-b0f8-32221b831e00"
            }
          ]
        },
        {
          "id": "bf2f12f7-b2b2-45d6-adf7-e8a5e2ac9fda",
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
              "id": "b9a2b37b-5863-4b16-b8f2-577cc131d2c5"
            }
          ]
        },
        {
          "id": "c2e18511-677b-4d40-b94a-9001eec549fa",
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
              "id": "fe43988c-eb69-4f2a-a237-8e792c377839"
            }
          ]
        },
        {
          "id": "4da5102b-80b3-4bbe-8e23-1ad21b7c0cbf",
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
              "id": "5506056f-ab39-4672-9b83-fb1ef8bb3a48"
            }
          ]
        }
      ]
    }
  ]
}