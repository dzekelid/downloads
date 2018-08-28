---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Enforcement Case
    Search Enforcement Case Download Data Service
  description: Based on the QID obtained from a get_cases query, return a comma sepated
    vaule (CSV) file of the cases found.
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 1.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /echo_rest_services.get_download:
    get:
      summary: Combined ECHO Download Data Service
      description: Based on the QID obtained from a get_facilities or get_facility_info
        query, return a comma sepated vaule (CSV) file of the facilities found.
      operationId: based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va
      x-api-path-slug: echo-rest-services-get-download-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Combined
      - ECHO
      - Download
      - Data
      - Service
  /air_rest_services.get_download:
    get:
      summary: Clean Air Act Download Data Service
      description: Based on the QID obtained from a get_facilities or get_facility_info
        query, return a comma sepated vaule (CSV) file of the facilities found.
      operationId: based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va
      x-api-path-slug: air-rest-services-get-download-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Air
      - Act
      - Download
      - Data
      - Service
  /cwa_rest_services.get_geojson:
    get:
      summary: Clean Water Act (CWA) Download Data Service
      description: Based on the QID obtained from a get_facilities or get_facility_info
        query, return a comma sepated vaule (CSV) file of the facilities found.
      operationId: based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va
      x-api-path-slug: cwa-rest-services-get-geojson-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Water
      - Act
      - (CWA)
      - Download
      - Data
      - Service
  /eff_rest_services.download_effluent_chart:
    get:
      summary: Effluent Charts Download Service
      description: Downloads tabular Discharge Monitoring Report (DMR) and compliance
        data for one NPDES permit as a CSV.
      operationId: downloads-tabular-discharge-monitoring-report-dmr-and-compliance-data-for-one-npdes-permit-as-a-csv-
      x-api-path-slug: eff-rest-services-download-effluent-chart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Effluent
      - Charts
      - Download
      - Service
  /case_rest_services.get_download:
    get:
      summary: Enforcement Case Download Data Service
      description: Based on the QID obtained from a get_cases query, return a comma
        sepated vaule (CSV) file of the cases found.
      operationId: based-on-the-qid-obtained-from-a-get-cases-query-return-a-comma-sepated-vaule-csv-file-of-the-cases-
      x-api-path-slug: case-rest-services-get-download-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Enforcement
      - Case
      - Download
      - Data
      - Service
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