---
name: HERE
x-slug: here
description: HERE Technologies enables people, enterprises and cities around the world
  to harness the power of location and create innovative solutions that make our lives
  safer and more efficient. We transform information from devices, vehicles, infrastructure
  and...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
x-kinRank: "7"
x-alexaRank: "3011"
tags: Addresses
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/apis.md
specificationVersion: "0.14"
apis:
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-openapi.md
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-openapi.md
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-openapi.md
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-openapi.md
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-openapi.md
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/here/geocode-json-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://developer.here.com/blog/feed
- type: x-github
  url: https://github.com/heremaps
- type: x-postman-collection
  url: https://github.com/heremaps/postman-collections
- type: x-api-gallery
  url: http://healthcare.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://here.stack.network
- type: x-blog
  url: https://developer.here.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/here-inc
- type: x-developer
  url: https://developer.here.com
- type: x-email
  url: dirk.popp@here.com
- type: x-email
  url: sebastian.kurme@here.com
- type: x-email
  url: jordan.stark@here.com
- type: x-email
  url: amy.stupavsky@here.com
- type: x-email
  url: minna.laub@here.com
- type: x-email
  url: stefanie.sirc@here.com
- type: x-email
  url: rachel.kuta@here.com
- type: x-email
  url: laurel.davis-lyons@here.com
- type: x-email
  url: linda.bradley@here.com
- type: x-email
  url: press@here.com
- type: x-twitter
  url: https://twitter.com/here
- type: x-website
  url: https://here.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---