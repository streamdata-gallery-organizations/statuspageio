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
  /pages/[page_id]/incidents/[incident_id]/incident_updates/[incident_update_id].json:
    patch:
      summary: Tune an Incident Update
      description: Tune an Incident Update
      operationId: tune-an-incident-update
      parameters:
      - in: query
        name: incident_update[body]
        description: The body of the incident update (optional)
        type: string
      - in: query
        name: incident_update[display_at]
        description: The timestamp by which to display the incident update (optional)
        type: string
      responses:
        200:
          description: OK
      tags:
      - incidents
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