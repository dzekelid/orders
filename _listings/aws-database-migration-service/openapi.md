swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeOrderableReplicationInstances:
    get:
      summary: Describe Orderable Replication Instances
      description: Returns information about the replication instance types that can
        be created in the specified region.
      operationId: describeOrderableReplicationInstances
      x-api-path-slug: actiondescribeorderablereplicationinstances-get
      parameters:
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances