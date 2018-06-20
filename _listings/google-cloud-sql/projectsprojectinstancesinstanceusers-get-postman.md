{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Users",
    "_postman_id": "6b7c43be-51a7-425b-887d-ce7be1a29039",
    "description": "Lists users in the specified Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "5df429d4-c605-4948-b157-ae99353b8bd2",
          "name": "sql.users.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/users"
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
            "description": "Lists users in the specified Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d324a97e-3c06-4530-b802-25025d8d5016"
            }
          ]
        }
      ]
    }
  ]
}