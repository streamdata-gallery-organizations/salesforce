{
  "info": {
    "name": "Salesforce Sandbox Get Version",
    "_postman_id": "9878986c-ab11-4243-ad9a-7028b6c75a91",
    "description": "Lists available resources for the specified API version, including resource name and URI.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "417bfb1a-bc62-439b-9544-04e2ba4d507d",
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
              "id": "f534764b-6099-430c-9fbf-efa25fd7de57"
            }
          ]
        }
      ]
    },
    {
      "name": "Version",
      "item": [
        {
          "id": "20c1b0fa-d84f-4360-9f47-dcfa297cb60d",
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
              "id": "64111fed-7109-4532-a032-6e6b28a1915b"
            }
          ]
        }
      ]
    }
  ]
}