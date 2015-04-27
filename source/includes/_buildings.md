# Buildings

> Definition

```
GET /api/buildings/{bin}
```

> Example Request

```shell
curl "/api/buildings/12345678"
```

> Example Response

```json
{
	"bbl": null,
	"bin": "1018131",
	"health_area": "5300",
	"census_tract": "68",
	"community_board": "105",
	"buildings_on_lot": "1",
	"tax_block": "882",
	"condo": "NO",
	"vacant": "NO",
	"cross_streets": "EAST   26 STREET,   EAST   27 STREET",
	"dob_special_place_name": "",
	"landmark_status": "",
	"local_law": "YES",
	"environmental_restrictions": "N/A",
	"legal_adult_use": "NO",
	"loft_law": "NO",
	"special_status": "N/A",
	"city_owned": "NO",
	"special_district": "UNKNOWN",
	"complaints": {
		"total": "33",
		"open": "0"
	},
	"violations": {
		"dob_total": "50",
		"dob_open": "2",
		"ecb_total": "14",
		"ecb_open": "4"
	}
}
```

Buildings are the primary resource for the NYC Buildings Api. They are queried using the BIN or Building Identification Number. If you don't have the BIN for the building you want to query, make sure to use the [helper endpoint](#helper)

