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
  /pages/[page_id]/page_access_users/[page_access_user_id]/components.json:
    post:
      summary: Assign components to a page access user (overwrites existing components)
      description: Assign components to a page access user (overwrites existing components)
      operationId: assign-components-to-a-page-access-user-overwrites-existing-components
      parameters:
      - in: query
        name: component_ids[]
        description: Array of component ids that the user will ba able to view
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