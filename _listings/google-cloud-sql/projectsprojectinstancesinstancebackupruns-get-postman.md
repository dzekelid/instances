{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Backupruns",
    "_postman_id": "df9f0eab-0467-4a7d-b726-2bd7724f8278",
    "description": "Lists all backup runs associated with a given instance and configuration in the reverse chronological order of the enqueued time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "001e934d-21d2-4ee3-8949-49ff53983358",
          "name": "sql.backupRuns.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/backupRuns"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all backup runs associated with a given instance and configuration in the reverse chronological order of the enqueued time"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b3532fa-e047-4dbf-a684-82d12e085c5d"
            }
          ]
        }
      ]
    }
  ]
}