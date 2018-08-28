{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Sslcerts",
    "_postman_id": "f7750731-c30c-4599-a53d-826a90378c3d",
    "description": "Lists all of the current SSL certificates for the instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "0661b5d6-ef30-4578-9499-6f1fc0c800d8",
          "name": "sql.sslCerts.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/sslCerts"
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
            "description": "Lists all of the current SSL certificates for the instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c433435d-e34c-468e-b65e-8d919bd7829f"
            }
          ]
        }
      ]
    }
  ]
}