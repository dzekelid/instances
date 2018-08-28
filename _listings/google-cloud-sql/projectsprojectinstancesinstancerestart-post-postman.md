{
  "info": {
    "name": "Google Cloud SQL API Add Projects Project Instances Instance Restart",
    "_postman_id": "8ca1fce2-e177-4676-928d-46c070fed835",
    "description": "Restarts a Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "0d7bb907-b396-416a-8d73-528f053a8381",
          "name": "sql.instances.restart",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/restart"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Restarts a Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dae4fe81-9180-4c98-bb2d-ed83821da46b"
            }
          ]
        }
      ]
    }
  ]
}