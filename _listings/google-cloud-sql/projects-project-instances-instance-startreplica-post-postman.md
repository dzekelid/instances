{
  "info": {
    "name": "Google Cloud SQL API Add Projects Project Instances Instance Startreplica",
    "_postman_id": "cbc3fab0-0cbe-4027-8245-6b83d5a7ac2c",
    "description": "Starts the replication in the read replica instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "911e67a6-55c9-4345-b5e3-cf75b300bf3b",
          "name": "sql.instances.startReplica",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/startReplica"
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
            "description": "Starts the replication in the read replica instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47b1846a-94a3-42d5-a24e-0d77592f48b4"
            }
          ]
        }
      ]
    }
  ]
}