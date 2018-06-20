{
  "info": {
    "name": "Salesforce Sandbox Get",
    "_postman_id": "ceca781c-5780-4fe3-930e-731b4e8e2558",
    "description": "Lists summary information about each Salesforce version currently available, including the version, label, and a link to each version's root.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "af24d127-02be-42aa-a3dc-aa07ac75fcf0",
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
          "id": "f07bd7b8-55e5-4a33-8852-00c2a1904779"
        }
      ]
    }
  ]
}