swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 1
info:
  title: AXA Assistance
  description: axa-assistance-is-a-worldwide-specialist-for-car-insurance-travel-health-and-home-services--trust-in-axa-assistance-for-your-insurance
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sales/v1/individual/appliance/certificates:
    post:
      summary: Requests the activation of a certificate either to cover an appliance
        purchased or to extend the warranty period of an appliance purchased. At least
        one product_criteria has to be specified to identify the product to which
        to subscribe. This endpoint
      description: Requests the activation of a certificate either to cover an appliance
        purchased or to extend the warranty period of an appliance purchased. At least
        one product_criteria has to be specified to identify the product to which
        to subscribe. This endpoint
      operationId: postSalesV1IndividualApplianceCertificates
      x-api-path-slug: salesv1individualappliancecertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - ofcertificate
      - either
      - to
      - coverappliance
      - purchasedto
      - extend
      - the
      - warranty
      - period
      - ofappliance
      - purchased.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - ThiAssistance
      - endpoint
  /sales/v1/individual/car_rental/certificates:
    post:
      summary: Requests the activation of a car rental certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal infor
      description: Requests the activation of a car rental certificate linked to a
        product. At least one product_criteria has to be specified to identify the
        product to which to subscribe. If the user already holds a certificate, this
        api will update its personal infor
      operationId: postSalesV1IndividualCar_rentalCertificates
      x-api-path-slug: salesv1individualcar-rentalcertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - ofcar
      - rental
      - certificate
      - linked
      - toproduct.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - If
      - the
      - user
      - already
      - holdscertificate
      - ""
      - thiAssistance
      - api
      - will
      - update
      - itAssistance
      - personal
      - infor
  /sales/v1/individual/travel/certificates:
    post:
      summary: Requests the activation of a travel certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal informati
      description: Requests the activation of a travel certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal informati
      operationId: postSalesV1IndividualTravelCertificates
      x-api-path-slug: salesv1individualtravelcertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - oftravel
      - certificate
      - linked
      - toproduct.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - If
      - the
      - user
      - already
      - holdscertificate
      - ""
      - thiAssistance
      - api
      - will
      - update
      - itAssistance
      - personal
      - informati