```json
{
"processInfo": {
	"cpid": "string", // from Path request parameter 'cpid'   
	"ocid": "string" // from Path request parameter 'ocid'
      },
"requestInfo": {
	"operationId": "string", // replace value from header
	"timeStamp": "string", // generate by controler
	"platformId": "uuid", // from Auth-token
	"owner": "uuid", // from Authorization header
	"token": "uuid" // from X-TOKEN header
	 },
"tender": { // generate
        "lots"[{
            "id": "uuid" //from Path request parameter 'lotId'   
           }],
		"amendments": [{ // from data
            "id": "uuid",
			"rationale": "string",
			"description": "string",
			"documents": [{
				"documentType": "cancellationDetails",
				"id": "835b8d03-80dc-4d1b-8b1c-fe2b1a23366c-1573211196021",
				"title": "string",
				"description": "string"
			}]
		}]
	}	
}
```
