{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance",
    "_postman_id": "bb5d1896-2839-4023-8096-ebfde0e55a6a",
    "description": "Retrieves a resource containing information about a Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "c085d09a-6249-442f-9328-a210d8b65d51",
          "name": "sql.instances.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance"
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
            "description": "Retrieves a resource containing information about a Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48b16f14-c462-4d30-afe9-012e55230c2f"
            }
          ]
        }
      ]
    }
  ]
}