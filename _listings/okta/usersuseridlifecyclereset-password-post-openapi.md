---
swagger: "2.0"
x-collection-name: Okta
x-complete: 0
info:
  title: Okta Reset Password
  description: Reset password.
  version: 1.0.0
host: example.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userId}:
    put:
      summary: Set Password
      description: Set password.
      operationId: putUsersUser
      x-api-path-slug: usersuserid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Password
  /users:
    get:
      summary: List Password Expired Users
      description: List password expired users.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: limit
      responses:
        200:
          description: OK
      tags:
      - List
      - Password
      - Expired
      - Users
  /users/{userId}/credentials/forgot_password:
    post:
      summary: Forgot Password (One Time Code)
      description: Forgot password (one time code).
      operationId: postUsersUserCredentialsForgotPassword
      x-api-path-slug: usersuseridcredentialsforgot-password-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: sendEmail
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Forgot
      - Password
      - (One
      - Time
      - Code)
  /users/{userId}/credentials/change_password:
    post:
      summary: Change Password
      description: Change password.
      operationId: postUsersUserCredentialsChangePassword
      x-api-path-slug: usersuseridcredentialschange-password-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Password
  /users/{userId}/lifecycle/reset_password:
    post:
      summary: Reset Password
      description: Reset password.
      operationId: postUsersUserLifecycleResetPassword
      x-api-path-slug: usersuseridlifecyclereset-password-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: sendEmail
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Reset
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