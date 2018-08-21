{
  "info": {
    "name": "SendGrid Get Devices Stats",
    "_postman_id": "6b5f27bd-e83c-4c44-be49-09e5e27623e0",
    "description": "**This endpoint allows you to retrieve your email statistics segmented by the device type.**\n\n**We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.\n\n## Available Device Types\n| **Device** | **Description** | **Example** |\n|---|---|---|\n| Desktop | Email software on desktop computer. | I.E., Outlook, Sparrow, or Apple Mail. |\n| Webmail |\tA web-based email client. | I.E., Yahoo, Google, AOL, or Outlook.com. |\n| Phone | A smart phone. | iPhone, Android, Blackberry, etc.\n| Tablet | A tablet computer. | iPad, android based tablet, etc. |\n| Other | An unrecognized device. |\n\nAdvanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "bc545a39-05b1-473a-b060-d7b0fba01b32",
          "name": "devices.stats.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/devices/stats?aggregated_by=%7B%7D&end_date=%7B%7D&limit=%7B%7D&No Name=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve your email statistics segmented by the device type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec700f18-00d8-4386-8c6b-48cb4eeac326"
            }
          ]
        }
      ]
    }
  ]
}