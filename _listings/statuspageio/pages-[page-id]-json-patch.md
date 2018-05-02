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
  /pages/[page_id].json:
    patch:
      summary: Update your page profile
      description: Update your page profile
      operationId: update-your-page-profile
      parameters:
      - in: query
        name: basic layout only, 170x45 or 340x90 is best
        type: string
      - in: query
        name: page[allow_email_subscribers]
        description: allow users to subscribe for email updates (t or f)
        type: string
      - in: query
        name: page[allow_incident_subscribers]
        description: allow users to subscribe to a single incident (t or f)
        type: string
      - in: query
        name: page[allow_page_subscribers]
        description: allow users to auto
        type: string
      - in: query
        name: page[allow_sms_subscribers]
        description: allow users to subscribe for sms updates (t or f)
        type: string
      - in: query
        name: page[city]
        description: city in which your page is headquartered
        type: string
      - in: query
        name: page[country]
        description: country in which your page is headquartered
        type: string
      - in: query
        name: page[css_body_background_color]
        description: custom css color for your status page body background
        type: string
      - in: query
        name: page[css_font_color]
        description: custom css color for your status page font
        type: string
      - in: query
        name: page[css_greens]
        description: custom css color for your status page greens
        type: string
      - in: query
        name: page[css_light_font_color]
        description: custom css color for your status page light font
        type: string
      - in: query
        name: page[css_oranges]
        description: custom css color for your status page oranges
        type: string
      - in: query
        name: page[css_reds]
        description: custom css color for your status page reds
        type: string
      - in: query
        name: page[css_yellows]
        description: custom css color for your status page yellows
        type: string
      - in: query
        name: page[domain]
        description: CNAME alias for your status page (point DNS record to hosted
        type: string
      - in: query
        name: page[hero_cover_url]
        description: url of a hero cover image to be placed on your status page
        type: string
      - in: query
        name: page[layout]
        description: which layout format to use for your status page
        type: string
      - in: query
        name: page[name]
        description: name of your page to be displayed
        type: string
      - in: query
        name: page[notifications_from_email]
        description: if users reply to the incident notifications we send
        type: string
      - in: query
        name: page[state]
        description: state in which your page is headquartered
        type: string
      - in: query
        name: page[subdomain]
        description: subdomain at which to access your status page (your_subdomain
        type: string
      - in: query
        name: page[time_zone]
        description: time zone to use for your status page display (must be a rails
          time zone)
        type: string
      - in: query
        name: page[transactional_logo_url]
        description: url of a transactional logo to be placed on your status page
        type: string
      - in: query
        name: page[url]
        description: the website of your page
        type: string
      - in: query
        name: premium layout only, 850x315 or 1700x630 is best
        type: string
      responses:
        200:
          description: OK
      tags:
      - pages
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