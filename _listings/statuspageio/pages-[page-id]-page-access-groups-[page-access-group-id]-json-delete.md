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
  /pages/[page_id]/page_access_groups/[page_access_group_id].json:
    delete:
      summary: Delete a group
      description: Delete a group
      operationId: delete-a-group
      parameters:
      - in: query
        name: page_access_group[orphan_mode]
        description: specifies what to do with any associated PageAccessUsers that
          are members of the group
        type: string
      responses:
        200:
          description: OK
      tags:
      - page access group
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