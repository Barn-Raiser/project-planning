# Phase 1
## Request 
```
mutation {
  createNeed(
              point_of_contact: "string value"
              description: "string value"
              start_time: "string value"
              end_time: "string value"
              street_address: "string value"
              city: "string value"
              state: "string value"
              zip_code: "string value"
              requested_supporters: int_value
            )
 }
```

# Phase 2
## Request
```
mutation {
  createNeed(
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

## Response
```
  # TODO: check on format for response
    "categories": ["", "", ""]
```
