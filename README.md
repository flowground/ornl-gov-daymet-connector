# ![LOGO](logo.png) Daymet Single Pixel Tool **flow**ground Connector

## Description

A generated **flow**ground connector for the Daymet Single Pixel Tool API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/ornl.gov/daymet/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:29+03:00

## API Description

Welcome to the Daymet Single Pixel Tool API. You can use this API to download daily surface data within the Daymet database in a `csv` or `json` format for a single point. This API allows users to query a single geographic point by latitude and longitude in decimal degrees. A routine is executed that translates the (lon, lat) coordinates into projected Daymet (x,y) Lambert Conformal Coordinates. These coordinates are used to access the Daymet database of daily interpolated surface weather variables. Daily data from the nearest 1 km x 1 km Daymet grid cell are extracted from the database.

If you would like to learn how to automate the download of multiple locations for the Daymet Single Pixel Tool, click [here](https://github.com/ornldaac/daymet-single-pixel-batch).

## Authorization

This API does not require authorization.

## Actions

### Download Daymet Data

> Returns a csv or json of the requested data to local machine

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `vars` - _optional_ - Daymet Daily weather estimates.
* `years` - _optional_ - Subset on years [1980..2017].
* `start` - _optional_ - Subset on dates (start date).
* `end` - _optional_ - Subset on dates (end date).
* `format` - _required_ - Specify a format for data retrieval.
    Possible values: csv, json.

### Preview Daymet Data in a web browser

> Returns a table to the browser displaying requested data

#### Input Parameters
* `lat` - _required_ - Latitude component of location
* `lon` - _required_ - Longitude component of location.
* `vars` - _optional_ - Daymet Daily weather estimates.
* `years` - _optional_ - Subset on years [1980..2016].
* `start` - _optional_ - Subset on dates (start date).
* `end` - _optional_ - Subset on dates (end date).
* `format` - _required_ - Specify a format for data retrieval.
    Possible values: csv, json.

### Download Daymet Data

> Returns a csv or json of the requested data to local machine

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `vars` - _optional_ - Daymet Daily weather estimates.
* `years` - _optional_ - Subset on years [1980..2016].
* `start` - _optional_ - Subset on dates (start date).
* `end` - _optional_ - Subset on dates (end date).
* `format` - _required_ - Specify a format for data retrieval.
    Possible values: csv, json.

### Visualize Daymet Data in a web browser

> Returns plots to a web browser of requested data using Plotly

#### Input Parameters
* `lat` - _required_ - Latitude component of location.
* `lon` - _required_ - Longitude component of location.
* `vars` - _optional_ - Daymet Daily weather estimates.
* `years` - _optional_ - Subset on years [1980..2016].
* `start` - _optional_ - Subset on dates (start date).
* `end` - _optional_ - Subset on dates (end date).
* `format` - _required_ - Specify a format for data retrieval.
    Possible values: csv, json.

## License

**flow**ground :- Telekom iPaaS / ornl-gov-daymet-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
