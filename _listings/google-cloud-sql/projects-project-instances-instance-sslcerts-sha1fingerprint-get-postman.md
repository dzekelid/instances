{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Sslcerts Sha1fingerprint",
    "_postman_id": "fda111aa-8eab-4060-baf2-fbbf2775e128",
    "description": "Retrieves a particular SSL certificate. Does not include the private key (required for usage). The private key must be saved from the response to initial creation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "039fd952-b522-4e59-af1a-6969936bba70",
          "name": "sql.sslCerts.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a particular SSL certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4130490-3fcd-42ac-9024-9d9d99868cba"
            }
          ]
        }
      ]
    }
  ]
}