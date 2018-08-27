{
  "info": {
    "name": "Dezrez Deletes the item stored at {itemKey}",
    "_postman_id": "d011967f-923b-4c23-b736-4183499e5102",
    "description": "Deletes the item stored at {itemkey}.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "S",
      "item": [
        {
          "id": "ef5ef6ee-91ea-4abd-a728-729c95e3ae85",
          "name": "Cache_DeleteItemByitemKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/cache/:itemKey"
              ],
              "variable": [
                {
                  "id": "itemKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the item stored at {itemkey}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86cfa5da-1cb9-4466-93ce-1aedb156760c"
            }
          ]
        }
      ]
    }
  ]
}