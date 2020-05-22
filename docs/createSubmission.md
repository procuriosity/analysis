```json
{
	"submissions": { // generate
     "details": [{ // generate
		"id": "string", // from request.payload.submission.id
		"requirementResponses": [{ // from request.payload.submission.requirementResponses
			"id": "string",
			"value": true, // or string or number or integer
			"requirement": {
				"id": "string"
			},
			"relatedCandidate": { // from request.payload.submission.requirementResponses[*].relatedCandidate
                "name":"", 
				"id": "" /* concatenate request.payload.submission.requirementResponses[*].relatedCandidate.identifier.scheme 
                            + request.payload.submission.requirementResponses[*].relatedCandidate.identifier.id  */
			}
		}],
		"candidates": [{  // from request.payload.submission.candidates
			"id": "string",  /* concatenate  request.payload.submission.candidates[*].identifier.scheme 
                                + request.payload.submission.candidates[*].identifier.id  */
			"name": "string",
			"identifier": {
				"id": "string",
				"legalName": "string",
				"scheme": "string",
				"uri": "string"
			},
			"additionalIdentifiers": [{
				"id": "string",
				"legalName": "string",
				"scheme": "string",
				"uri": "string"
			}],
			"address": {
				"streetAddress": "string",
				"postalCode": "string",
				"addressDetails": {
					"country": {
						"id": "string",
						"description": "string",
						"scheme": "string",
						"uri": "string"
					},
					"region": {
						"id": "string",
						"description": "string",
						"scheme": "string",
						"uri": "string"
					},
					"locality": {
						"id": "string",
						"description": "string",
						"scheme": "string",
						"uri": "string"
					}
				}
			},
			"contactPoint": {
				"name": "string",
				"email": "string",
				"telephone": "string",
				"faxNumber": "string",
				"url": "string"
			},
			"persones": [{
                "id": "string",  /* concatenate  request.payload.submission.candidates[*].persones[*].identifier.scheme 
                                + request.payload.submission.candidates[*].persones[*].identifier.id  */
				"title": "string",
				"name": "string",
				"identifier": {
					"scheme": "string",
					"id": "string",
					"uri": "string"
				},
				"businessFunctions": [{
					"id": "string",
					"type": "chairman",
					"jobTitle": "string",
					"period": {
						"startDate": "2020-05-04T15:16:05.947Z"
					},
					"documents": [{
						"id": "string",
						"documentType": "regulatoryDocument",
						"title": "string",
						"description": "string"
					}]
				}]
			}]
		}],
            "details": {
                "typeOfSupplier": "company",
                "mainEconomicActivity": [{
                    "scheme": "MD-CAE      M",
                    "id": "string",
                    "description": "string",
                    "uri": "string"
                }],
                "scale": "micro",
                "bankAccounts": [
                {
                  "description": "string",
                  "bankName": "string",
                  "address": {
                    "streetAddress": "string",
                    "postalCode": "string",
                    "addressDetails": {
                      "country": {
                        "id": "string",
                        "description": "string",
                        "scheme": "string"
                      },
                      "region": {
                        "id": "string",
                        "description": "string",
                        "scheme": "string"
                      },
                      "locality": {
                        "id": "string",
                        "description": "string",
                        "scheme": "string"
                      }
                    }
                  },
                  "identifier": {
                    "scheme": "UA-MFO",
                    "id": "string"
                  },
                  "accountIdentification": {
                    "scheme": "IBAN",
                    "id": "string"
                  },
                  "additionalAccountIdentifiers": [
                    {
                      "scheme": "fiscal",
                      "id": "string"
                    }
                  ]
                }
          ],
                "legalForm": {
                   "scheme": "MD-CFOJ",
                   "id": "string",
                   "description": "string",
                   "uri": "string"
          }
        }
      }
    ],
		"documents": [{ // from request.payload.submission.documents
			"id": "string",
			"documentType": "regulatoryDocument",
			"title": "string",
			"description": "string"
		}]
	}]}
}
```