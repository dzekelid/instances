{
  "info": {
    "name": "Google Cloud SQL API Add Projects Project Instances Instance Promotereplica",
    "_postman_id": "a7e1f09c-5a8e-48b9-9ffd-aa8192be2fe2",
    "description": "Promotes the read replica instance to be a stand-alone Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "da3bdc50-3541-42d5-a7f7-b0f7eaf2b4d6",
          "name": "sql.instances.promoteReplica",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/promoteReplica"
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
            "description": "Promotes the read replica instance to be a stand-alone Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7917932-9b5a-4da0-989c-ee9501719592"
            }
          ]
        }
      ]
    }
  ]
}