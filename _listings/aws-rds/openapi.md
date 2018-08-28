swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeOrderableDBInstanceOptions:
    get:
      summary: Describe Orderable D B Instance Options
      description: Returns a list of orderable DB instance options for the specified
        engine.
      operationId: describeorderabledbinstanceoptions
      x-api-path-slug: actiondescribeorderabledbinstanceoptions-get
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Engine
        description: The name of the engine to retrieve DB instance options for
        type: string
      - in: query
        name: EngineVersion
        description: The engine version filter value
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: LicenseModel
        description: The license model filter value
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeOrderableDBInstanceOptions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Vpc
        description: The VPC filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances