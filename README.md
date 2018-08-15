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
3. ## [Static]
4. ## [Uploads]
5. ## [Datasets]
6. ## [Tilequery]
7. ## [Tilesets]
8. ## [Geocoding]
9. ## [Directions]
10. ## [Map Matching]
11. ## [Matrix]
12. ## [Optimization]
13. ## [Tokens]
14. ## [Analytics]



# REST APIs
The Mapbox web services APIs allow for programmatic access to Mapbox tools and services. Use these APIs to retrieve information about your account, upload and change resources, and use core Mapbox tools, like geocoding and directions.

## Maps
The Mapbox Maps API supports reading raster tilesets, vector tilesets, and Mapbox Editor project features. Tilesets can be retrieved as images, TileJSON, or HTML slippy maps for embedding. Mapbox Editor project features can be retrieved as GeoJSON or KML.

1. ###  **Retrieve tiles** - Returns a image tile, vector tile, or UTFGrid in the specified format.
2. ###  **Retrieve an HTML slippy map** - Returns an HTML slippy map for sharing or embedding.
3. ###  **Retrieve features from Mapbox Editor projects** - Retrieve vector features from Mapbox Editor projects as GeoJSON or KML. GeoJSON returns a FeatureCollection with features that conform to the simplestyle-spec
4. ###  **Retrieve TileJSON metadata** - Returns TileJSON metadata for a tileset. This is an object that describes a map's resources, like tiles, markers, and UTFGrid, as well as its name, description, and centerpoint.
5. ### **Retrieve a standalone marker** - Request a single marker? image without any background map.

[MAPS End Points - RUN IN POSTMAN](https://documenter.getpostman.com/view/5039671/RWTmvJda)                      
[MAPS API Endpoints Collection - Download](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Maps.postman_collection.json)


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

[STYLES End Points - RUN IN POSTMAN](https://documenter.getpostman.com/view/5039671/RWTmvJhv)                      
[STYLES API Endpoints Collection - Download](https://github.com/umer-ali-khan/mapbox-postman-collections/blob/master/MapBox%20-%20Styles.postman_collection.json)
