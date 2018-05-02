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
  /pages/[page_id]/page_access_groups.json:
    post:
      summary: Create a group that will define what and who can view elements of your
        status page
      description: Create a group that will define what and who can view elements
        of your status page
      operationId: create-a-group-that-will-define-what-and-who-can-view-elements-of-your-status-page
      parameters:
      - in: query
        name: page_access_group[component_ids][]
        description: Array of component ids that the created group will be able to
          view
        type: string
      - in: query
        name: page_access_group[external_identifier]
        description: A unique string that can be used to associate this group with
          an external group (optional)
        type: string
      - in: query
        name: page_access_group[metric_ids][]
        description: Array of metric ids that the created group will be able to view
        type: string
      - in: query
        name: page_access_group[name]
        description: The name the group (required)
        type: string
      - in: query
        name: page_access_group[page_access_user_ids][]
        description: Array of Page Access User ids that the created group contain
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