---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Places Get Shape History
  description: Return an historical list of all the shape data generated for a Places
    or Where on Earth (WOE) ID.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.places.find:
    get:
      summary: Places Find
      description: Return a list of place IDs for a query string.
      operationId: getRestMethodFlickr.places.find
      x-api-path-slug: restmethodflickr-places-find-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: query
        description: The query string to use for place ID lookups
      responses:
        200:
          description: OK
      tags:
      - Places
      - Find
  /rest/?method=flickr.places.findByLatLon:
    get:
      summary: Places Find By Lat Lon
      description: Return a place ID for a latitude, longitude and accuracy triple.
      operationId: getRestMethodFlickr.places.findbylatlon
      x-api-path-slug: restmethodflickr-places-findbylatlon-get
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the location information
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: lat
        description: The latitude whose valid range is -90 to 90
      - in: query
        name: lon
        description: The longitude whose valid range is -180 to 180
      responses:
        200:
          description: OK
      tags:
      - Places
      - FindByLatLon
  /rest/?method=flickr.places.getChildrenWithPhotosPublic:
    get:
      summary: Places Get Children With Photos Public
      description: Return a list of locations with public photos that are parented
        by a Where on Earth (WOE) or Places ID.
      operationId: getRestMethodFlickr.places.getchildrenwithphotospublic
      x-api-path-slug: restmethodflickr-places-getchildrenwithphotospublic-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where On Earth (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetChildrenWithPhotosPublic
  /rest/?method=flickr.places.getInfo:
    get:
      summary: Places Get Info
      description: Get information about a place.
      operationId: getRestMethodFlickr.places.getinfo
      x-api-path-slug: restmethodflickr-places-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where On Earth (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetInfo
  /rest/?method=flickr.places.getInfoByUrl:
    get:
      summary: Places Get Info By Url
      description: Lookup information about a place, by its flickr.com/places URL.
      operationId: getRestMethodFlickr.places.getinfobyurl
      x-api-path-slug: restmethodflickr-places-getinfobyurl-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: url
        description: A flickr
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetInfoByUrl
  /rest/?method=flickr.places.getPlaceTypes:
    get:
      summary: Places Get Place Types
      description: Fetches a list of available place types for Flickr.
      operationId: getRestMethodFlickr.places.getplacetypes
      x-api-path-slug: restmethodflickr-places-getplacetypes-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetPlaceTypes
  /rest/?method=flickr.places.getShapeHistory:
    get:
      summary: Places Get Shape History
      description: Return an historical list of all the shape data generated for a
        Places or Where on Earth (WOE) ID.
      operationId: getRestMethodFlickr.places.getshapehistory
      x-api-path-slug: restmethodflickr-places-getshapehistory-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where On Earth (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetShapeHistory
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