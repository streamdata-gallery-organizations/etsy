---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Countries Country
  description: Retrieves a Country by id.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /countries/{country_id}:
    get:
      summary: Get Countries Country
      description: Retrieves a Country by id.
      operationId: getCountriesCountry
      x-api-path-slug: countriescountry-id-get
      parameters:
      - in: path
        name: country_id
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Country
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