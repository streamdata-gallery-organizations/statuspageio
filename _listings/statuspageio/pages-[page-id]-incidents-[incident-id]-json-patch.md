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
  /pages/[page_id]/incidents/[incident_id].json:
    patch:
      summary: Update an incident (only applies to realtime and scheduled incidents)
      description: Update an incident (only applies to realtime and scheduled incidents)
      operationId: update-an-incident-only-applies-to-realtime-and-scheduled-incidents
      parameters:
      - in: query
        name: at the same time to avoid two separate incident updates being generated.
        type: string
      - in: query
        name: ENDPOINT
        type: string
      - in: query
        name: incident[component_ids]
        description: List of components whose subscribers should be notified (only
          applicable for pages with component subscriptions enabled)
        type: string
      - in: query
        name: incident[impact_override]
        description: Override calculated impact value, one of none|minor|major|critical
          (optional)
        type: string
      - in: query
        name: incident[message]
        description: The body of the new incident update that will be created (optional)
        type: string
      - in: query
        name: incident[name]
        description: The name of the incident
        type: string
      - in: query
        name: incident[status]
        description: The status, one of investigating|identified|monitoring|resolved
          (if realtime) or scheduled|in_progress|verifying|completed (if scheduled)
        type: string
      - in: query
        name: incident[wants_twitter_update]
        description: Post the new incident update to twitter (t or f, defaults to
          f)
        type: string
      - in: query
        name: MUTABLE
        type: string
      - in: query
        name: PATCH /pages/[page_id]/incidents/[incident_id].json
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