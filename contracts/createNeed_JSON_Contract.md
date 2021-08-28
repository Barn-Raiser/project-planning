# Phase 1
## Request 
```
mutation {
  createNeed(input:
    	     {
              pointOfContact: "string value"
   	      title: "This is a new need"
              description: "string value"
              startTime: "string value"
              endTime: "string value"
              streetAddress: "string value"
              city: "string value"
              state: "string value"
              zipCode: "string value"
              supportersNeeded: 12
            }
            )
  {
    need {
          id
          title
          description  
          pointOfContact
          startTime 
          endTime 
          zipCode 
          supportersNeeded 
          status
        }
    errors
	}
}
```

## Response (with requested data returned)
```
{
  "data": {
    "createNeed": {
      "need": {
        "id": "19",
        "title": "This is a new need",
        "description": "string value",
        "pointOfContact": "string value",
        "startTime": "string value",
        "endTime": "string value",
        "zipCode": "string value",
        "supportersNeeded": 12,
        "status": 0
      },
      "errors": []
    }
  }
}
```

# Phase 2
## Request
```
mutation {
  createNeed(input: 
              point_of_contact: "string value"
              description: "string value"
              start_time: "string value"
              end_time: "string value"
              street_address: "string value"
              city: "string value"
              state: "string value"
              zip_code: "string value"
              requested_supporters: int_value
              categories: ["", ""]
            )
            # TODO: CHECK ON FORMAT FOR response request 
            {
            categories
            }
 }
```

```
mutation {
  createNeed(input:
    				{
              pointOfContact: "string value"
   						title: "This is a new need"
              description: "string value"
              startTime: "string value"
              endTime: "string value"
              streetAddress: "string value"
              city: "string value"
              state: "string value"
              zipCode: "string value"
              supportersNeeded: 12
              categories: ["", ""]
            }
            )
  {
    need {
          id
          title
          description  
          pointOfContact
          startTime 
          endTime 
          zipCode 
          supportersNeeded 
          status
          categories
        }
  errors
	}
}
```

## Response
```
{
  "data": {
    "createNeed": {
      "need": {
        "id": "19",
        "title": "This is a new need",
        "description": "string value",
        "pointOfContact": "string value",
        "startTime": "string value",
        "endTime": "string value",
        "zipCode": "string value",
        "supportersNeeded": 12,
        "status": 0
        "categories": ["", ""]
      },
      "errors": []
    }
  }
}
```
