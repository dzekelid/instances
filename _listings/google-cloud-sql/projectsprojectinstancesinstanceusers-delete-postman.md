{
  "info": {
    "name": "Google Cloud SQL API Delete Projects Project Instances Instance Users",
    "_postman_id": "e62cb2c7-5406-4707-9aff-06ea702e1881",
    "description": "Deletes a user from a Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "1be8403e-fd5e-450f-a2d4-875b03127a56",
          "name": "sql.users.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/users"
              ],
              "query": [
                {
                  "key": "host",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Deletes a user from a Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb4f654a-4b8a-4781-a5fe-d851eaf17d81"
            }
          ]
        }
      ]
    }
  ]
}