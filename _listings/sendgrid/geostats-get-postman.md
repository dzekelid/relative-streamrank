{
  "info": {
    "name": "SendGrid Get Geo Stats",
    "_postman_id": "d85c45fe-f0c5-4a5a-a1e4-ae648f3b3711",
    "description": "**This endpoint allows you to retrieve your email statistics segmented by country and state/province.**\n\n**We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.\n\nAdvanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "7395e953-e612-42bf-a857-a21e9f0fde37",
          "name": "geo.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/geo/stats?aggregated_by=%7B%7D&country=%7B%7D&end_date=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your email statistics segmented by country and state/province"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc9d0716-ed7e-4f0c-bb3f-abfefcfebc17"
            }
          ]
        }
      ]
    }
  ]
}