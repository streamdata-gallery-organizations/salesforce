{
  "info": {
    "name": "SalesForce Get Version",
    "_postman_id": "03b50e5d-1033-4d86-84fe-b44cd2cd471a",
    "description": "Lists available resources for the specified API version, including resource name and URI.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "6ed77c3b-1333-4c9a-b5a5-77f9c04a2fde",
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
              "id": "3f87df74-9911-4fae-94c9-e5001c01b39c"
            }
          ]
        }
      ]
    }
  ]
}