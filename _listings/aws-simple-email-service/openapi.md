swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 1
info:
  title: AWS Simple Email Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListVerifiedEmailAddresses:
    get:
      summary: List Verified Email Addresses
      description: Returns a list containing all of the email addresses that have
        been verified.
      operationId: listVerifiedEmailAddresses
      x-api-path-slug: actionlistverifiedemailaddresses-get
      parameters:
      - in: query
        name: VerifiedEmailAddresses.member.N
        description: A list of email addresses that have been verified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verified Email Addresses
  /?Action=DeleteVerifiedEmailAddress:
    get:
      summary: Delete Verified Email Address
      description: Deletes the specified email address from the list of verified addresses.
      operationId: deleteVerifiedEmailAddress
      x-api-path-slug: actiondeleteverifiedemailaddress-get
      parameters:
      - in: query
        name: EmailAddress
        description: An email address to be removed from the list of verified addresses
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verified Email Addresses
  /?Action=VerifyEmailAddress:
    get:
      summary: Verify Email Address
      description: Verifies an email address.
      operationId: verifyEmailAddress
      x-api-path-slug: actionverifyemailaddress-get
      parameters:
      - in: query
        name: EmailAddress
        description: The email address to be verified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Email Addresses