---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List address POS relations
  description: List address pos relations.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/addresses/{addressTypeId?}:
    get:
      summary: List addresses that are linked with contacts
      description: Lists addresses of the contact. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactAddressesAddresstype
      x-api-path-slug: restaccountscontactscontactidaddressesaddresstypeid-get
      parameters:
      - in: path
        name: addressTypeId?
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Addresses
      - That
      - Are
      - Linked
      - Contacts
  /rest/orders/{orderId}/addresses/{relationTypeId?}:
    get:
      summary: List order addresses
      description: Lists order addresses. The ID of the order must be specified.
      operationId: getRestOrdersOrderAddressesRelationtype
      x-api-path-slug: restordersorderidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: relationTypeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Addresses
  /rest/stockmanagement/warehouses/{warehouseId}/addresses/{relationTypeId?}:
    get:
      summary: List warehouse addresses
      description: List warehouse addresses. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseAddressesRelationtype
      x-api-path-slug: reststockmanagementwarehouseswarehouseidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: relationTypeId?
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Addresses
  /rest/accounts/addresses:
    post:
      summary: Create an address
      description: Create an address.
      operationId: postRestAccountsAddresses
      x-api-path-slug: restaccountsaddresses-post
      parameters:
      - in: body
        name: /rest/accounts/addresses
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
  /rest/accounts/addresses/contact_relations:
    get:
      summary: List address contact relations
      description: List address contact relations.
      operationId: getRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-get
      parameters:
      - in: query
        name: addressId
        description: Filter that restricts the search result to addresses with a specific
          ID
      - in: query
        name: contactId
        description: Filter that restricts the search result to contacts with a specific
          ID
      - in: query
        name: id
        description: Filter that restricts the search result to address contact relations
          with a specific ID
      - in: query
        name: isPrimary
        description: Filter that restricts the search result depending on the flag
          used
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: typeId
        description: Filter that restricts the search result to address types with
          a specific ID
      - in: query
        name: with
        description: Includes the specified address contact relation information in
          the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Contact
      - Relations
    post:
      summary: Create address contact relations
      description: Create address contact relations.
      operationId: postRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-post
      parameters:
      - in: body
        name: /rest/accounts/addresses/contact_relations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relations
    put:
      summary: Update address contact relations
      description: Update address contact relations.
      operationId: putRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/contact_relations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relations
  /rest/accounts/addresses/contact_relations/{addressContactRelationId}:
    delete:
      summary: Delete an address contact relation
      description: Deletes an address contact relation. The ID of the relation must
        be specified.
      operationId: deleteRestAccountsAddressesContactRelationsAddresscontactrelation
      x-api-path-slug: restaccountsaddressescontact-relationsaddresscontactrelationid-delete
      parameters:
      - in: path
        name: addressContactRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relation
    get:
      summary: Get an address contact relation
      description: Gets an address contact relation. The ID of the address contact
        relation must be specified.
      operationId: getRestAccountsAddressesContactRelationsAddresscontactrelation
      x-api-path-slug: restaccountsaddressescontact-relationsaddresscontactrelationid-get
      parameters:
      - in: path
        name: addressContactRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relation
  /rest/accounts/addresses/option_types:
    get:
      summary: List address option types
      description: List address option types.
      operationId: getRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Option
      - Types
    post:
      summary: Create an address option type
      description: Create an address option type.
      operationId: postRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-post
      parameters:
      - in: body
        name: /rest/accounts/addresses/option_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
  /rest/accounts/addresses/option_types/{optionTypeId}:
    delete:
      summary: Delete an address option type
      description: Deletes an address option type. The ID of the option type must
        be specified.
      operationId: deleteRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-delete
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
    get:
      summary: Get an address option type
      description: Gets an address option type. The ID of the option type must be
        specified.
      operationId: getRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-get
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
    put:
      summary: Update an address option type
      description: Updates an address option type. The ID of the option type must
        be specified.
      operationId: putRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/option_types/{optionTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
  /rest/accounts/addresses/options/{optionId}:
    delete:
      summary: Delete an address option by the option ID
      description: Deletes an address option. The ID of the option must be specified.
      operationId: deleteRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-delete
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - By
      - Option
      - ID
    get:
      summary: Get an address option
      description: Gets an address option. The ID of the option must be specified.
      operationId: getRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-get
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
    put:
      summary: Update an address option
      description: Updates an address option. The ID of the option must be specified.
      operationId: putRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-put
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
  /rest/accounts/addresses/pos_relations:
    get:
      summary: List address POS relations
      description: List address pos relations.
      operationId: getRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: items per page
      - in: query
        name: page
        description: page
      - in: query
        name: with
        description: Includes the specified address pos relation information in the
          results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - POS
      - Relations
    post:
      summary: Create an address POS relation
      description: Create an address pos relation.
      operationId: postRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-post
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
  /rest/accounts/addresses/pos_relations/{addressPosRelationId}:
    delete:
      summary: Delete an address POS relation
      description: Deletes an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: deleteRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-delete
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
    get:
      summary: Get an address POS relation
      description: Gets an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: getRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-get
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
    put:
      summary: Update an address POS relation
      description: Updates an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: putRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-put
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
  /rest/accounts/addresses/relation_types:
    get:
      summary: List address relation types
      description: List address relation types.
      operationId: getRestAccountsAddressesRelationTypes
      x-api-path-slug: restaccountsaddressesrelation-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/relations/types/applications/{application}/{lang}:
    get:
      summary: List address relation types
      description: |-
        Lists address relation types. The application and the language must be specified.
        <br>Possible applications:
        <ul>
        <li>contact</li>
        <li>order</li>
        <li>warehouse</li>
        <li>pos</li>
        </ul>
      operationId: getRestAccountsAddressesRelationsTypesApplicationsApplicationLang
      x-api-path-slug: restaccountsaddressesrelationstypesapplicationsapplicationlang-get
      parameters:
      - in: path
        name: application
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/warehouse_relations:
    post:
      summary: Create an address warehouse relation
      description: Create an address warehouse relation.
      operationId: postRestAccountsAddressesWarehouseRelations
      x-api-path-slug: restaccountsaddresseswarehouse-relations-post
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
  /rest/accounts/addresses/warehouse_relations/{relationId}:
    delete:
      summary: Delete an address warehouse relation
      description: Deletes an address warehouse relation. The ID of the relation must
        be specified.
      operationId: deleteRestAccountsAddressesWarehouseRelationsRelation
      x-api-path-slug: restaccountsaddresseswarehouse-relationsrelationid-delete
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
    put:
      summary: Update an address warehouse relation
      description: Updates an address warehouse relation. The ID of the relation must
        be specified.
      operationId: putRestAccountsAddressesWarehouseRelationsRelation
      x-api-path-slug: restaccountsaddresseswarehouse-relationsrelationid-put
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
  /rest/accounts/addresses/{addressId}:
    delete:
      summary: Delete an address
      description: Deletes an address. The ID of the address must be specified.
      operationId: deleteRestAccountsAddressesAddress
      x-api-path-slug: restaccountsaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
    get:
      summary: Get an address
      description: Gets an address. The ID of the address must be specified.
      operationId: getRestAccountsAddressesAddress
      x-api-path-slug: restaccountsaddressesaddressid-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
    put:
      summary: Update an address
      description: Updates an address. The ID of the address must be specified.
      operationId: putRestAccountsAddressesAddress
      x-api-path-slug: restaccountsaddressesaddressid-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/{addressId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
  /rest/accounts/addresses/{addressId}/options:
    delete:
      summary: Delete an address option by the address ID
      description: Deletes an address option. The ID of the address must be specified.
      operationId: deleteRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-delete
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - By
      - Address
      - ID
    get:
      summary: List address options
      description: Lists address options. The ID of the address must be specified.
      operationId: getRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Options
    post:
      summary: Create an address option
      description: Creates an address option. The ID of the address must be specified.
      operationId: postRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-post
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
    put:
      summary: Update the address options for an address
      description: Update the address options for an address.
      operationId: putRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-put
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Optionsan
      - Address
  /rest/accounts/addresses/{addressId}/related_data:
    get:
      summary: Find address data by address id
      description: Find address data by address id.
      operationId: getRestAccountsAddressesAddressRelatedData
      x-api-path-slug: restaccountsaddressesaddressidrelated-data-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Address
      - Data
      - By
      - Address
      - Id
  /rest/accounts/contacts/{contactId}/addresses/{addressId}:
    delete:
      summary: Delete an address of the contact
      description: Deletes an address of the contact. The ID of the contact and the
        ID of the address must be specified.
      operationId: deleteRestAccountsContactsContactAddressesAddress
      x-api-path-slug: restaccountscontactscontactidaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      - in: path
        name: contactId
      - in: query
        name: typeId
        description: The type ID of the address
      responses:
        200:
          description: OK
      tags:
      - Address
      - Of
      - Contact
    put:
      summary: Update an address of the contact
      description: Updates an address of the contact. The ID of the contact and the
        ID of the address must be specified.
      operationId: putRestAccountsContactsContactAddressesAddress
      x-api-path-slug: restaccountscontactscontactidaddressesaddressid-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: contactId
      - in: query
        name: isPrimary
        description: Sets a contact address per address type as the primary address
      - in: query
        name: typeId
        description: The type ID of the address
      responses:
        200:
          description: OK
      tags:
      - Address
      - Of
      - Contact
  /rest/accounts/contacts/{contactId}/addresses/{addressId}/types/{addressTypeId}/primary:
    put:
      summary: Set a contact address per address type as the primary address
      description: Sets a contact address per address type as the primary address.
        The ID of the contact, the ID of the address and the ID of the address type
        must be specified. A primary address is also definable if you create or update
        a contact address.
      operationId: putRestAccountsContactsContactAddressesAddressTypesAddresstypePrimary
      x-api-path-slug: restaccountscontactscontactidaddressesaddressidtypesaddresstypeidprimary-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: addressTypeId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Contact
      - Address
      - Per
      - Address
      - Type
      - As
      - Primary
      - Address
  /rest/accounts/contacts/{contactId}/addresses/{addressId}/types/{addressTypeId}/reset_primary:
    put:
      summary: Resets a contact primary address
      description: Resets a contact primary address. The ID of the contact, the ID
        of the address and the ID of the address type must be specified.
      operationId: putRestAccountsContactsContactAddressesAddressTypesAddresstypeResetPrimary
      x-api-path-slug: restaccountscontactscontactidaddressesaddressidtypesaddresstypeidreset-primary-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: addressTypeId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Resets
      - Contact
      - Primary
      - Address
  /rest/accounts/order_summaries/orders/{addressId}:
    get:
      summary: Get an order summary by the address ID
      description: Gets an order summary. The ID of the address must be specified.
      operationId: getRestAccountsOrderSummariesOrdersAddress
      x-api-path-slug: restaccountsorder-summariesordersaddressid-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Address
      - ID
  /rest/accounts/contacts/{contactId}/addresses:
    post:
      summary: Create an address for existing contact and type
      description: Creates an address. The ID of the contact must be specified.
      operationId: postRestAccountsContactsContactAddresses
      x-api-path-slug: restaccountscontactscontactidaddresses-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/{contactId}/addresses
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactId
      - in: query
        name: isPrimary
        description: Sets a contact address per address type as the primary address
      - in: query
        name: typeId
        description: The type ID of the address
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Contact
      - Type
  /rest/orders/addresses:
    post:
      summary: Create an address for existing order
      description: Creates an address for an existing order.
      operationId: postRestOrdersAddresses
      x-api-path-slug: restordersaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Order
  /rest/stockmanagement/warehouses/addresses:
    post:
      summary: Create an address for existing warehouse
      description: Create an address for existing warehouse.
      operationId: postRestStockmanagementWarehousesAddresses
      x-api-path-slug: reststockmanagementwarehousesaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Warehouse
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