swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeOrderableClusterOptions:
    get:
      summary: Describe Orderable Cluster Options
      description: Returns a list of orderable cluster options.
      operationId: describeOrderableClusterOptions
      x-api-path-slug: actiondescribeorderableclusteroptions-get
      parameters:
      - in: query
        name: ClusterVersion
        description: The version filter value
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: NodeType
        description: The node type filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Options