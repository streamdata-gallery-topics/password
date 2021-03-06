---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Resets user password by username
  version: 1.0.0
  description: Resets user password by username.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/password:
    patch:
      summary: Resets user password by userid
      description: Resets user password by userid.
      operationId: resetPasswordById
      x-api-path-slug: usersuseridpassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Password
      - By
      - Userid
  /users/by-username/{username}/password:
    patch:
      summary: Resets user password by username
      description: Resets user password by username.
      operationId: resetPasswordByUsername
      x-api-path-slug: usersbyusernameusernamepassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Password
      - By
      - Username
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