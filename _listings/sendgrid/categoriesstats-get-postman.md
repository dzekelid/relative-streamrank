{
  "info": {
    "name": "SendGrid Get Categories Stats",
    "_postman_id": "0ae67ccd-eb25-4d81-9965-cd09ecf1f82b",
    "description": "**This endpoint allows you to retrieve all of your email statistics for each of your categories.**\n\nIf you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.\n\nCategories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "ae7a5491-9a6a-4a0d-9ee8-982a13512d1d",
          "name": "categories.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/categories/stats?aggregated_by=%7B%7D&categories=%7B%7D&end_date=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of your email statistics for each of your categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "691418fb-674a-40b1-8e53-dbc889ac20f1"
            }
          ]
        }
      ]
    }
  ]
}