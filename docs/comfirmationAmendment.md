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
        "amendments": [{ // from data
           "id": "uuid" // from Path requests parameter amendmentId
           }]
    }
}
```