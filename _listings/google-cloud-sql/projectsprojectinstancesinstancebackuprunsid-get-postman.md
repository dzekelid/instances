{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Backupruns",
    "_postman_id": "4e1560a5-78e1-45db-a81c-251afadbc607",
    "description": "Retrieves a resource containing information about a backup run.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "f8e74e03-6967-402b-8abb-f88ec61ca651",
          "name": "sql.backupRuns.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a resource containing information about a backup run"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9035da53-ffb0-4435-b181-934d989aa0f4"
            }
          ]
        }
      ]
    }
  ]
}