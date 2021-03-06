---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Put User Password
  description: |-
    **This endpoint allows you to update your password.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/password:
    put:
      summary: Put User Password
      description: |-
        **This endpoint allows you to update your password.**

        Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

        For more information about your user profile:

        * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
      operationId: user.password.put
      x-api-path-slug: userpassword-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Password
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---