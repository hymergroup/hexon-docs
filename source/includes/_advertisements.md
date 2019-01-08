# Advertisements

## Create an Advertisement


```shell
curl "https://staging.financial.leasedesk.nl/api/v1/advertisement/create
    -X POST
    -H "Authorization: Bearer <your_access_token>"
    -H "Content-Type: application/json"
    -H "Accept: application/json"
    --data {
        "name": "Autobedrijf Janssen",
        "image_src": "Stationstraat",
        "target_url": "10",
        "display_from": "",
        "display_to": "",
        "show_in_brands": [
        	"1",
        	"2"
        ],
        "show_in_type": [
        	"1",
        	"2"
        ],        
    }
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 1,
        "name": "Autobedrijf Janssen",
        "img_src": "Stationstraat",
        "target_url": "10",
        "display_to": "",
        "show_in_brands": [
        	"1",
        	"2"
        ],
        "show_in_type": [
        	"1",
        	"2"
        ],   
    }
}
```
This endpoint creates a new Advertisement. An advertisement can be given dates in which the advertisement will be shown.
An advertisement can be specific for one or more brands, and/or, one or more types ( models ).

<aside class="warning">Make sure you send the json payload as raw body data to the endpoint.</aside>

### HTTP Request

`POST https://staging.financial.leasedesk.nl/api/v1/advertiser/create`

### Raw Body Parameters (JSON)

Parameter | Description | Required | Validation Rules
--------- | ----------- | -------- | ----------------
name | Name of the Advertisement | yes | *none*
image_src | Absolute source of the advertisement image | yes | *valid URL*
target_url | Absolute Target of the advertisement | yes | *valid URL*
display_from | date from which the advertisement should be visible | no | *date:Y-m-d*
display_to | date to which the advertisement should not be visible | no | *date:Y-m-d*
show_in_brands | array of brand_ID's in which this advertisement should be shown | no | *array*
show_in_type | array of type_ID's in which this advertisement should be shown | no | *array*

## Delete a Specific Advertisement

```shell
curl "https://staging.financial.leasedesk.nl/api/v1/advertisement/1"
  -X DELETE
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
[]
```

This endpoint deletes a specific Advertisement.

<aside class="warning">The JSON response will be empty, when the Advertisement is deleted succesfully a HTTP 200 OK response will be returned.</aside>

### HTTP Request

`DELETE https://staging.financial.leasedesk.nl/api/v1/advertisement/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the advertisement to delete