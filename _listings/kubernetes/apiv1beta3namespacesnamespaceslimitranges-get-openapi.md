---
swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 0
info:
  title: Kubernetes Get Namespaces Limitranges
  version: 1.0.0
  description: List objects of kind limitrange.
host: /api/v1beta3
basePath: 127.0.0.1:6443
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1beta3/limitranges:
    get:
      summary: Get Limitranges
      description: List objects of kind limitrange.
      operationId: listLimitRange
      x-api-path-slug: apiv1beta3limitranges-get
      responses:
        200:
          description: OK
      tags:
      - Limitranges
  /api/v1beta3/namespaces/{namespaces}/limitranges:
    get:
      summary: Get Namespaces Limitranges
      description: List objects of kind limitrange.
      operationId: listLimitRange
      x-api-path-slug: apiv1beta3namespacesnamespaceslimitranges-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Limitranges
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