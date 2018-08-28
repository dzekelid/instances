{
  "info": {
    "name": "Google Cloud SQL API Add Projects Project Instances Instance Stopreplica",
    "_postman_id": "67ee0f0e-2ab7-4268-8ee0-85748ed74671",
    "description": "Stops the replication in the read replica instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "7b2bbfbe-fe07-4a57-871c-fd657ad35ae3",
          "name": "sql.instances.stopReplica",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/stopReplica"
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
            "description": "Stops the replication in the read replica instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "058713bb-3915-4033-8e7d-fd6422e07005"
            }
          ]
        }
      ]
    }
  ]
}