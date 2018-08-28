{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances",
    "_postman_id": "1cb3f8c4-2794-469e-bd08-2306a415fb2d",
    "description": "Lists instances under a given project in the alphabetical order of the instance name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "0dc31e21-51d8-4dcf-8713-308d8fe84393",
          "name": "sql.instances.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "description": "Lists instances under a given project in the alphabetical order of the instance name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09d741b4-c620-49b1-8d53-cca9c0f646ae"
            }
          ]
        }
      ]
    }
  ]
}