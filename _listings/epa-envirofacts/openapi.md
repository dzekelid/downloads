swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 1
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking
    Water Act
  description: enforcement-and-compliance-history-online-echo-is-a-tool-developed-and-maintained-by-epas-office-of-enforcement-and-compliance-assurance-for-public-use--echo-provides-integrated-compliance-and-enforcement-information-for-about-800000-regulated-facilities-nationwide-brbrsdw-rest-services-provides-multiple-service-endpoints-each-with-specific-capabilities-to-search-and-retrieve-data-on-public-water-systems-regulated-under-the-safe-drinking-water-act-sdwa--the-returned-results-reflect-data-drawn-from-epas-federal-safe-drinking-water-information-system-sdwis-database-brbrthe-get-systems-get-qid-and-get-download-end-points-are-meant-to-be-used-together-brbrthe-recommended-use-scenario-for-get-systems-get-qid-and-get-downoad-isbrbrb1bnbsp-use-get-systems-to-validate-passed-query-parameters-obtain-summary-statistics-and-to-obtain-a-query-id-qid---qids-are-time-sensitive-and-will-be-valid-for-approximately-30-minutes-brb2bnbsp-use-get-qid-with-the-returned-qid-to-paginate-through-arrays-of-water-system-results-brb3bnbsp-use-get-download-with-the-returned-qid-to-generate-a-comma-separated-value-csv-file-of-water-system-information-that-meets-the-qid-query-criteria-brbruse-the-qcolumns-parameter-to-customize-your-search-results---use-the-metdata-service-endpoint-for-a-list-of-available-output-objects-their-column-ids-and-their-definitions-to-help-you-build-your-customized-output--brbradditional-echo-resourcesnbspnbsp-a-hrefhttpsecho-epa-govtoolswebservicesweb-servicesa-a-hrefhttpsecho-epa-govresourcesechodataaboutthedataabout-echos-dataa-a-hrefhttpsecho-epa-govtoolsdatadownloadsdata-downloadsabr
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
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
  /rcra_rest_services.get_download:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Download Data Service
      description: Based on the QID obtained from a get_facilities or get_facility_info
        query, return a comma sepated vaule (CSV) file of the facilities found.
      operationId: based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va
      x-api-path-slug: rcra-rest-services-get-download-get
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
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Download
      - Data
      - Service
  /sdw_rest_services.get_download:
    get:
      summary: Safe Drinking Water Act (SDWA) Download Data Service
      description: Based on the QID obtained from a get_systems query, return a comma
        sepated vaule (CSV) file of the water systems found.
      operationId: based-on-the-qid-obtained-from-a-get-systems-query-return-a-comma-sepated-vaule-csv-file-of-the-wate
      x-api-path-slug: sdw-rest-services-get-download-get
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
      - Safe
      - Drinking
      - Water
      - Act
      - (SDWA)
      - Download
      - Data
      - Service