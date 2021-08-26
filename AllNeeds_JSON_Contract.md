### Request: 

```
{ allActiveNeeds 
  {
    point_of_contact
    description
    start_time 
    end_time 
    zip_code 
    requested_supporters 
  }
}
```
    
### Response: 
```
{ "allActiveNeeds": 
  [
    { "point_of_contact": "string_value",
      "description": "string_value",
      "start_time: "string_value",
      "end_time ": "string_value",
      "zip_code": "string_value",
      "requested_supporters": int_value },
     { "point_of_contact": "string_value",
      "description": "string_value",
      "start_time: "string_value",
      "end_time ": "string_value",
      "zip_code": "string_value",
      "requested_supporters": int_value },
     { "point_of_contact": "string_value",
      "description": "string_value",
      "start_time: "string_value",
      "end_time ": "string_value",
      "zip_code": "string_value",
      "requested_supporters": int_value }
  ]
}
```
