# Complaints

> Definition

```
GET /api/complaints/{complaint_num}
```

> Example Request

```shell
curl "/api/buildings/12345678/complaints"
```

> Example Response

```json
{
	"bin": "3036607",
	"complaint_num": "3058960",
	"regarding": "Re: ILLEGAL PLUMBING WORK IN BASEMENT/CELLAR",
	"category": "66 PLUMBING WORK - ILLEGAL/NO PERMIT(ALSO SPRINKLER/STANDPIPE)",
	"assigned_to": "",
	"priority": "",
	"received": "10/01/1997 11:28",
	"block": " 1374",
	"lot": " 31",
	"community_board": " 308",
	"owner": "REQ 74104 00000002257970",
	"last_inspection": "06/05/2003 - - BY BADGE # 3029",
	"disposition": "06/06/2003 - I2 - NO VIOLATION WARRANTED FOR COMPLAINT AT TIME OF INSPECTION",
	"dob_violation_num": "NO FUTHER ACTION NECESSARY BASED UPON PHYSICAL OBSERVATION",
	"ecb_violation_num": "",
	"comments": ""
}
```

Description of complaints endpoint


## Building Complaints

> Definition

```
GET /api/buildings/{bin}/complaints
```

> Example Request

```shell
curl "/api/buildings/12345678/complaints"
```

> Example Response

```json
[
	{
		"bin": "3036607",
		"complaint_num": "3058960",
		"regarding": "Re: ILLEGAL PLUMBING WORK IN BASEMENT/CELLAR",
		"category": "66 PLUMBING WORK - ILLEGAL/NO PERMIT(ALSO SPRINKLER/STANDPIPE)",
		"assigned_to": "",
		"priority": "",
		"received": "10/01/1997 11:28",
		"block": " 1374",
		"lot": " 31",
		"community_board": " 308",
		"owner": "REQ 74104 00000002257970",
		"last_inspection": "06/05/2003 - - BY BADGE # 3029",
		"disposition": "06/06/2003 - I2 - NO VIOLATION WARRANTED FOR COMPLAINT AT TIME OF INSPECTION",
		"dob_violation_num": "NO FUTHER ACTION NECESSARY BASED UPON PHYSICAL OBSERVATION",
		"ecb_violation_num": "",
		"comments": ""
	}
]
```