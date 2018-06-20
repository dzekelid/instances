{
  "info": {
    "name": "Google Cloud SQL API Delete Projects Project Instances Instance",
    "_postman_id": "0dfa4697-6d15-4246-b6dd-f660cd328ed1",
    "description": "Deletes a Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "cdff31ed-24ee-428c-9de4-f72a7576d0d0",
          "name": "sql.instances.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance"
              ],
              "variable": [
                {
                  "id": "instance",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ae6d1be-28c9-4a28-beb3-360aad044840"
            }
          ]
        }
      ]
    }
  ]
}