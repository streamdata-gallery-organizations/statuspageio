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
  /pages/[page_id]/components/[component_id]/page_access_groups.json:
    post:
      summary: Assign page access groups to a component
      description: Assign page access groups to a component
      operationId: assign-page-access-groups-to-a-component
      parameters:
      - in: query
        name: page_access_group_ids[]
        description: Array of page access group ids for groups that can access the
          referenced component
        type: string
      responses:
        200:
          description: OK
      tags:
      - page access users
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