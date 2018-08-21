---
swagger: "2.0"
x-collection-name: Paylocity
x-complete: 0
info:
  title: Paylocity Get Earnings by Earning Code
  description: Get Earnings returns all earnings with the provided earning code for
    the selected employee.
  termsOfService: WebLink.OpenApiDoc.TermsOfService
  version: "2"
host: api.paylocity.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/companies/{companyId}/employees/{employeeId}/earnings:
    get:
      summary: Get All Earnings
      description: Get All Earnings returns all earnings for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearnings-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
  /v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}:
    get:
      summary: Get Earnings by Earning Code
      description: Get Earnings returns all earnings with the provided earning code
        for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcode-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
      - EarningCode
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---