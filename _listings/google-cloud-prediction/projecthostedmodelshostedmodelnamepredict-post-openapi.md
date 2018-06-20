---
swagger: "2.0"
x-collection-name: Google Cloud Prediction
x-complete: 0
info:
  title: Google Cloud Prediction API Predict Model
  description: Submit input and request an output against a hosted model.
  contact:
    name: Google
    url: https://google.com
  version: v1.6
host: www.googleapis.com
basePath: /prediction/v1.6/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/hostedmodels/{hostedModelName}/predict:
    post:
      summary: Predict Model
      description: Submit input and request an output against a hosted model.
      operationId: prediction.hostedmodels.predict
      x-api-path-slug: projecthostedmodelshostedmodelnamepredict-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: hostedModelName
        description: The name of a hosted model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
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