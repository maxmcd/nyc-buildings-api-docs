# Helper

> Definition

```
GET /api/helper/{params}
```

> Example Request

```shell
curl "/api/helper/?BBL=121212"
```

> Example Response

```json
{
    "bin":"12341234",
    "bbl":"121212",
    "address":"adsfsadf"
}
```


Buildings in NYC can be queried using multiple different identifiers. We primarily use the BBL identifier, but provide a helper endpoint to return identifiers from multiple inputs.

Because of the diverse set of possible inputs for this endpoint there are 5 parameter groups that can be used. They are:

 - `bin`
 - `bbl`
 - `address`
 - `borough`, `block` & `lot`
 - `borough`, `number` & `street`

### Query Parameters

Parameter | Description
--------- | -----------
bin |  The Building Identification Number
bbl |  Building Block and Lot number. The number is occasionally padded with zeros. The api will try and parse it correctly but it's recommended to use the separare `borough` `block` and `lot` params instead.
address | Pass a full address and the api will attempt to parse it and return building information. This is the least constent input parameter for this endpoint and relies on the strength of geocoding.
borough | The borough number
block | The block number
lot | The lot number
number | The street number of the building
street | The street name

