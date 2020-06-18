```json
"qualifications": // generate
	[{
		"id": "uuid", //from Path qualificationId parameter
		"requirementResponses": //from Data
		[{
			"id": "string",
			"value": true,
			"relatedTenderer": {
				"id": "string"
			},
			"responder": {
				"title": "string",
				"name": "string",
				"identifier": {
					"scheme": "string",
					"id": "string",
					"uri": "string"
				},
				"businessFunctions": [{
					"id": "string",
					"type": "enum",
					"jobTitle": "string",
					"period": {
						"startDate": "date-time"
					},
					"documents": [{
						"id": "string",
						"documentType": "enum",
						"title": "string",
						"description": "string"
					}]
				}]
			},
			"requirement": {
				"id": "string" 
			}]
		}
	}]
}
```
