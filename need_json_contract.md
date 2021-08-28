### Request: get info on one need, identified by ID number 

```
{ need(id:1) 
  {
    title
    description  
    pointOfContact
    startTime 
    endTime 
    zipCode 
    supportersNeeded 
    status
  }
}
```

### Successful response should look like

```
{
    "data": {
        "need": {
            "title": "This is a new need",
            "description": "string value",
            "pointOfContact": "string value",
            "startTime": "string value",
            "endTime": "string value",
            "zipCode": "string value",
            "supportersNeeded": 12,
            "status": "active"
        }
    }
}
```
