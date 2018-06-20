---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API List model runs for a particular model.
  description: List the model runs for a particular model, 20 per page.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /model:
    get:
      summary: List models.
      description: List the models, 20 per page.
      operationId: list-the-models-20-per-page
      x-api-path-slug: model-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the models
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Models
  /model/{model_identifier}:
    get:
      summary: Get a representation of a model.
      description: Get JSON which represents the structure of a model.
      operationId: get-json-which-represents-the-structure-of-a-model
      x-api-path-slug: modelmodel-identifier-get
      parameters:
      - in: path
        name: model_identifier
        description: model_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Model
  /model/{model_identifier}/run:
    get:
      summary: List model runs for a particular model.
      description: List the model runs for a particular model, 20 per page.
      operationId: list-the-model-runs-for-a-particular-model-20-per-page
      x-api-path-slug: modelmodel-identifierrun-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the model runs
      - in: path
        name: model_identifier
        description: model_identifier description
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Model
      - Runsa
      - Particular
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