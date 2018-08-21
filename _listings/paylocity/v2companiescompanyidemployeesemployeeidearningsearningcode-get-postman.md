{
  "info": {
    "name": "Paylocity Get Earnings by Earning Code",
    "_postman_id": "0ba60522-8f50-472a-9ba3-3b50e595736d",
    "description": "Get Earnings returns all earnings with the provided earning code for the selected employee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V2",
      "item": [
        {
          "id": "a0a7f924-d132-439a-bd17-dcac7f2048b2",
          "name": "v2.companies.companyId.employees.employeeId.earnings.earningCode.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.paylocity.com",
              "path": [
                "api",
                "v2/companies/:companyId/employees/:employeeId/earnings/:earningCode"
              ],
              "variable": [
                {
                  "id": "companyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "earningCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "employeeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer + JWT",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Earnings returns all earnings with the provided earning code for the selected employee."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69e45db8-25e4-468c-861c-a9933d7869e5"
            }
          ]
        }
      ]
    }
  ]
}