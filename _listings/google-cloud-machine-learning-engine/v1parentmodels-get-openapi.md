---
swagger: "2.0"
x-collection-name: Google Cloud Machine Learning Engine
x-complete: 0
info:
  title: Google Cloud Machine Learning API List Models
  description: |-
    Lists the models in a project.

    Each project can contain multiple models, and each model can have multiple
    versions.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: ml.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{parent}/models:
    get:
      summary: List Models
      description: |-
        Lists the models in a project.

        Each project can contain multiple models, and each model can have multiple
        versions.
      operationId: ml.projects.models.list
      x-api-path-slug: v1parentmodels-get
      parameters:
      - in: query
        name: pageSize
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: parent
        description: Required
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