```json
{
"processInfo": {
	"cpid": "string", // from Path request parameter "cpid"  
	"ocid": "string" // from Path request parameter "ocid"  
     },
"requestInfo": {
	"operationId": "string", // replace value from header
	"timeStamp": "string", // generate by controler
	"platformId": "uuid", // from Auth-token
    "owner": "uuid", // from Authorization header
    "token": "uuid" // from X-TOKEN header
	 }, 
"awards": // generate
	[{
		"id": "uuid", //from Path awardId parameter
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
				"id": "uuid" 
			}]
		}
	}]
}
```
