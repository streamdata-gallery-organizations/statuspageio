---
swagger: "2.0"
info:
  title: StatusPage.io
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages/[page_id]/metrics_providers/[metrics_provider_id]/metrics.json:
    get:
      summary: Get a list of metrics created for a linked metrics provider
      description: Get a list of metrics created for a linked metrics provider
      operationId: get-a-list-of-metrics-created-for-a-linked-metrics-provider
      responses:
        200:
          description: OK
      tags:
      - metric providers
definitions: []
x-collection-name: StatusPage.io
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