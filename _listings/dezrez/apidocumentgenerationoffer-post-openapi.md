---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a correspondence notifying the vendor of an offer.  Uses
    default values where possible.
  version: 1.0.0
  description: Generates a correspondence notifying the vendor of an offer.  uses
    default values where possible..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default agency brand if brandId
        is not supplied.
      description: Get a specific brand by brandid or default agency brand if brandid
        is not supplied..
      operationId: Agency_GetAgencyBrandByidBybrandId
      x-api-path-slug: apiagencyidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of an agency
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Agency
      - Brand
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/role/auction/milestone/{roleId}/create:
    put:
      summary: Create default milestones for role if they dont exist
      description: Create default milestones for role if they dont exist.
      operationId: AuctionRole_PopulateAuctionMilestonesByroleId
      x-api-path-slug: apiroleauctionmilestoneroleidcreate-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Milestonesrole
      - If
      - They
      - Dont
      - Exist
  /api/branch/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default brand within a branch if
        brandId is not supplied.
      description: Get a specific brand by brandid or default brand within a branch
        if brandid is not supplied..
      operationId: Branch_GetBranchBrandByidBybrandId
      x-api-path-slug: apibranchidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of a branch
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Brand
      - Within
      - Branch
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/documentgeneration/confirmvaluation:
    post:
      summary: Generates a correspondence confirming the booking of a valuation appointment.  Uses
        default values where possible.
      description: Generates a correspondence confirming the booking of a valuation
        appointment.  uses default values where possible..
      operationId: DocumentGeneration_GenerateValuationConfirmationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmvaluation-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Confirming
      - Booking
      - Of
      - Valuation
      - Appointment
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/valuationresult:
    post:
      summary: Generates a correspondence confirming the result of a valuation appointment.  Uses
        default values where possible.
      description: Generates a correspondence confirming the result of a valuation
        appointment.  uses default values where possible..
      operationId: DocumentGeneration_GenerateValuationResultLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvaluationresult-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Confirming
      - Result
      - Of
      - Valuation
      - Appointment
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offer:
    post:
      summary: Generates a correspondence notifying the vendor of an offer.  Uses
        default values where possible.
      description: Generates a correspondence notifying the vendor of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationoffer-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Notifying
      - Vendor
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
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