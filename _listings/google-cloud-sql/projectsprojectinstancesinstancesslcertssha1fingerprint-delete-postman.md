{
  "info": {
    "name": "Google Cloud SQL API Delete Projects Project Instances Instance Sslcerts Sha1fingerprint",
    "_postman_id": "07f91bd7-a8c3-4620-a9cd-6837d7a1b6a3",
    "description": "Deletes the SSL certificate. The change will not take effect until the instance is restarted.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "5715f509-2892-40e1-b1cb-bfdcc628b705",
          "name": "sql.sslCerts.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/sslCerts/:sha1Fingerprint"
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
                },
                {
                  "id": "sha1Fingerprint",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSL certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9b04c9b-173b-4eea-93eb-947d3bf84807"
            }
          ]
        }
      ]
    }
  ]
}