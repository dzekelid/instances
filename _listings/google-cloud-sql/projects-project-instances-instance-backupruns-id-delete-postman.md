{
  "info": {
    "name": "Google Cloud SQL API Delete Projects Project Instances Instance Backupruns",
    "_postman_id": "efd100f7-2c7e-4444-b69e-f47e0471472a",
    "description": "Deletes the backup taken by a backup run.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "bcdff9b4-6b9d-4e18-99bb-a7d081f13753",
          "name": "sql.backupRuns.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/backupRuns/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Deletes the backup taken by a backup run"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbfd6b8b-77f1-4d71-b9d3-23c68a17584a"
            }
          ]
        }
      ]
    }
  ]
}