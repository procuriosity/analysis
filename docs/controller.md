```json
{
"processInfo": {
    "cpid": "string", // from Path request parameter 'cpid'
    "ocid": "string" // from Path request parameter 'ocid'
     },
"requestInfo": {
	"operationId": "", // from X-OPERATION-ID header
	"timeStamp": "string", // generate by controler
    "requestId": "", // generate by controler
	"platformId": "uuid", // from Auth-token
    "owner": "string" // from Authorization header
    "token": "string" // form X-TOKEN header (if present)
   },
"request": {
    "id": "string", // from Path request parameter 'entityId'(if present)
    "payload": "string" // from Body (if present)
     }
}
```