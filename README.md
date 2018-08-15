# Mapbox-Postman-collections

Compiled and developed by Umar Ali Khan in cooperation with MapBox

This collection was produced in collaboration with Mapbox on 07-Aug-2018.

This repository holds a series of postman collections demonstrating a variety of use cases for all of the [MapBox Maps APIs](https://www.mapbox.com/api-documentation/).

These examples have been created for use with the Postman utility. Postman is a testing framework for REST APIs. The tool can be downloaded from www.getpostman.com.

To import the collection, first clone this repository, then open the Postman utility and select the Import option. Select the Folder tab from the dialog and drag and drop the cloned repository folder into the target.

The collections contained in this repository are organized under this scheme:

# [REST APIs](#rest-apis)
1. ## [Maps](#maps-1)
2. ## [Styles](#styles-1)
3. ## [Static](#static-1)
4. ## [Uploads](#uploads-1)
5. ## [Datasets](#datasets-1)
6. ## [Tilequery](#tilequery-1)
7. ## [Tilesets](#tilesets-1)
8. ## [Geocoding](#geocoding-1)
9. ## [Directions](#directions-1)
10. ## [Map Matching](#map-matching-1)
11. ## [Matrix](#matrix-1)
12. ## [Optimization](#optimization-1)
13. ## [Tokens](#tokens-1)
14. ## [Analytics](#analytics-1)



# REST APIs
The Mapbox web services APIs allow for programmatic access to Mapbox tools and services. Use these APIs to retrieve information about your account, upload and change resources, and use core Mapbox tools, like geocoding and directions.

## Maps
The Mapbox Maps API supports reading raster tilesets, vector tilesets, and Mapbox Editor project features. Tilesets can be retrieved as images, TileJSON, or HTML slippy maps for embedding. Mapbox Editor project features can be retrieved as GeoJSON or KML.

1. ###  **Retrieve tiles** - Returns a image tile, vector tile, or UTFGrid in the specified format.
2. ###  **Retrieve an HTML slippy map** - Returns an HTML slippy map for sharing or embedding.
3. ###  **Retrieve features from Mapbox Editor projects** - Retrieve vector features from Mapbox Editor projects as GeoJSON or KML. GeoJSON returns a FeatureCollection with features that conform to the simplestyle-spec
4. ###  **Retrieve TileJSON metadata** - Returns TileJSON metadata for a tileset. This is an object that describes a map's resources, like tiles, markers, and UTFGrid, as well as its name, description, and centerpoint.
5. ### **Retrieve a standalone marker** - Request a single marker? image without any background map.
[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJda)[![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Maps.postman_collection.json)


## Styles
The Mapbox Styles API lets you read and change map styles, fonts, and images. This API is the basis for Mapbox Studio, our cartography software.

1. ###  **List Styles** - Retrieve a list of styles for an account. This endpoint does not return full styles, but returns style metadata.
2. ###  **Create a style** - Creates a style in your account.
3. ###  **Update a Style** - Updates an existing style in your account with new content.
4. ###  **Delete a Style** - Deletes a style. All sprites that belong to this style will also be deleted, and the style will no longer be available.
5. ### **Retrieve font glyph ranges** - Glyph ranges are usually not of interest unless you're building a map renderer, but this is the endpoint where you can access them.
6. ### **Retrieve a sprite image or JSON** - Retrieves a sprite image or JSON document.
7. ### **Add new image to sprite** - Adds a new image to an existing sprite.
8. ### **Delete image from sprite** - Deletes an image from an existing sprite.
9. ### **Embed a Style** - Request embeddable HTML suitable for fullscreen map displays or for inserting into blog posts and articles as <iframe> content.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJhv)[![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Styles.postman_collection.json)


## Static
The Mapbox Static API returns static maps and raster tiles from styles in the Mapbox Style Specification. See the Static (Classic) API documentation.

Static maps are standalone images that can be displayed on web and mobile devices without the aid of a mapping library or API. They look like an embedded map without interactivity or controls.

1. ###  **Retrieve a static map from a style** - In contrast to the legacy Static API, this API supports pitch, bearing, and decimal zoom levels.
2. ###  **Retrieve raster tiles from styles** - Retrieve 512x512 or 256x256 pixel raster tiles from a Mapbox Studio style.
3. ###  **Retrieve a map's WMTS document** - Mapbox supports access via the WMTS standard, which lets you use maps with desktop and online GIS software like ArcMap and QGIS.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJhy)[![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Static.postman_collection.json)

## Uploads
The Mapbox Uploads API transforms geographic data into tilesets that can be used with maps and geographic applications. Given a wide variety of geospatial formats, it normalizes projections and generates tiles at multiple zoom levels to make data viewable on the web.

The upload workflow begins with a file and ends with a tileset?, or if you have invalid data, an error.

1. ###  **Retrieve S3 credentials** - Mapbox provides an Amazon S3 bucket to stage your file while your upload is processed. Uploads must be staged in this bucket before being uploaded to your Mapbox account. You can retrieve temporary credentials from this endpoint.
2. ###  **Create an upload** - Once you've used the temporary S3 credentials to transfer your file to Mapbox's staging bucket, you can trigger the generation of a tileset given the file's URL and a destination tileset ID.
3. ###  **Retrieve upload status** - Upload processing is fast but not immediate. Once an upload is created, you can track its status. Uploads have a progress property that will start at 0 and end at 1 when an upload is complete. If there's an error processing an upload, the error property will include an error message.
4. ###  **Retrieve recent upload statuses** - You can retrieve multiple upload statuses at the same time, sorted by the most recently created. This request returns the same information as individual upload status, but for all recent uploads. The list is limited to 1MB of JSON.
5. ###  **Remove an upload** - Remove a completed upload status from the upload listing.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJi1) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Uploads.postman_collection.json)

## Datasets
A dataset is an editable collection of GeoJSON features. The Datasets API offers persistent storage for custom geographic data and supports reading, creating, updating, and removing features. The goal of this API is to let you manage your geodata using Mapbox. To serve this data at scale, convert your dataset? into a tileset? using the Uploads API.

1. ###  **List datasets** - List datasets
2. ###  **Create dataset** - Creates a new, empty dataset
3. ###  **Retrieve a dataset** - Retrieve a dataset
4. ###  **Update a dataset** - Update a dataset
5. ###  **Delete a dataset** - Deletes a dataset, including all features it contains.
6. ###  **List features** - List features in a dataset?. The response body will be a GeoJSON FeatureCollection.
7. ###  **Insert or update a feature** - Inserts or updates a feature in a dataset. If there's already a feature with the given ID in the dataset, it will be replaced. If there isn't a feature with that ID, a new feature is created.
8. ###  **Retrieve a feature** - Retrieves a feature in a dataset.
9. ###  **Delete a feature** - Removes a feature from a dataset.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJnL)  [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Datasets.postman_collection.json)

## Tilequery
The Mapbox Tilequery API allows you to retrieve data about specific features from a vector tileset?, based on a given latitude and longitude?. With the Tilequery API, you can:

. Query for features within a given radius
. Do point in polygon queries
. Query multiple composited layers

1. ###  **Retrieve features from vector tiles** - The URL parameters for a request to the Mapbox Tilequery API are the map_id being queried and the specified {longitude}, {latitude} pair.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJnM)  [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Tilequery.postman_collection.json)

## Tilesets
The Mapbox Tilesets API supports reading metadata for raster and vector tilesets. To request tiles, consult the Maps API.

1. ###  **List tilesets** - Lists all tilesets for an account.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJnN) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Tilesets.postman_collection.json)

## Geocoding
The Mapbox Geocoding? API does two things: forward geocoding and reverse geocoding.

Forward geocoding lets you convert location text into geographic coordinates, turning 2 Lincoln Memorial Circle NW into -77.050,38.889.

1. ###  **Search for places** - This is often called forward geocoding. Request feature data that best matches the input {query} text. The response includes one or more results ordered by relevance.
2. ###  **Retrieve places near a location** - This is often called reverse geocoding. Request feature data located at the input {longitude},{latitude} coordinates. The response includes at most one result from each type, unless the limit parameter was used in the request.
3. ###  **Batch requests** - This feature is only available with the mapbox.places-permanent mode.
Batch requests have the same parameters as normal requests, but can include more than one query by separating queries with the ; character. Each query should be URL encoded, but the ; character should not be encoded and should be included verbatim.
4. ###  **POI categories** - POI category search supports forward geocoding? requests of poi feature types in a queried category. Using the proximity query parameter with POI category search returns points of interest local to a provided location; for example, restaurants near a user. Any category that is returned in the properties.category property of the response object is supported.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJnR) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Geocoding.postman_collection.json)

## Directions
The Mapbox Directions API will show you how to get where you're going. With the Directions API, you can:

. calculate optimal driving, walking, and cycling routes
. produce turn-by-turn instructions
. produce routes with up to 25 coordinates anywhere on earth


1. ###  **Retrieve directions** - Retrieve directions


[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJnS) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Directions.postman_collection.json)

## Map Matching
The Mapbox Map Matching API snaps fuzzy, inaccurate traces from a GPS unit or a phone to the OpenStreetMap? road and path network using the Directions API. This produces clean paths that can be displayed on a map or used for other analysis.

1. ###  **Retrieve a match** - Returns a path on the road and path network closest to the input traces.
2. ###  **Retrieve a match - Using HTTP POST** - Returns a path on the road and path network closest to the input traces.


[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJnT) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Map%20Matching.postman_collection.json)

## Matrix
The Matrix API returns travel times between many points.


1. ###  **Retrieve a matrix** - Returns a duration and/or distance matrix showing travel times and distances between coordinates.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJrj) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Matrix.postman_collection.json)

## Optimization
The Optimization API returns a duration-optimized route between the input coordinates. This is also known as solving the Traveling Salesperson Problem. A typical use case for this API is planning the route for deliveries in a city. A route can be retrieved for car driving, bicycling and walking or hiking.

1. ###  **Retrieve an optimization** - The {profile} parameter of your request should be a Mapbox Directions routing profile ID. The following IDs are supported:

. mapbox/driving for car trips
. mapbox/walking for pedestrian and hiking trips
. mapbox/cycling for bicycle trips

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJrm) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Optimization.postman_collection.json)

## Tokens
An access token, referred to hereafter as 'token', grants access to Mapbox resources on behalf of a user. All accounts have a public token by default. Additional tokens can be created to grant additional, or more limited, privileges.

1. ###  **List tokens** - Lists all tokens for an account.
2. ###  **Create token** - Creates a new token.
3. ###  **Create temporary token** - Creates a new temporary token that automatically expires at a fixed time.
4. ###  **Update a token** - Update note or scopes in a token's metadata.
5. ###  **Delete a token** - Revoke a token's authorization, removing its access to Mapbox APIs. This is the same as deleting a token. Applications using the revoked token will need to get a new access token? before they can access Mapbox APIs.
6. ###  **Retrieve a token** - Check if a token is valid. If the token is invalid an explanation of why is returned as the code property.
7. ###  **List scopes** - List scopes for a user. All potential scopes a user has access to are listed.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJrq) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Tokens.postman_collection.json)

## Analytics
The Mapbox Analytics API returns API usage for services by resource. For example, it can calculate the number of geocoding requests made in a week with a specific access token.

1. ###  **Retrieve analytics** - Returns the request counts per day for given resource and period.

[![](https://symbiotics.co.za/wp-content/uploads/2017/10/postman-logo.png)](https://documenter.getpostman.com/view/5039671/RWTmvJrs) [![](http://icons.iconarchive.com/icons/graphicloads/colorful-long-shadow/128/Arrow-download-icon.png)](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Analytics.postman_collection.json)
