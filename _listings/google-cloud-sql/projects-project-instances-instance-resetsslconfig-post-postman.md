{
  "info": {
    "name": "Google Cloud SQL API Add Projects Project Instances Instance Resetsslconfig",
    "_postman_id": "a53c74a1-7a29-4236-84f1-dcbde627aef5",
    "description": "Deletes all client certificates and generates a new server SSL certificate for the instance. The changes will not take effect until the instance is restarted. Existing instances without a server certificate will need to call this once to set a server certificate.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "625edc0d-25e2-403e-bfe4-83f849c60ae9",
          "name": "sql.instances.resetSslConfig",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/resetSslConfig"
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
            "description": "Deletes all client certificates and generates a new server SSL certificate for the instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3132e64a-25b5-48b6-a18b-73276ea98619"
            }
          ]
        }
      ]
    }
  ]
}