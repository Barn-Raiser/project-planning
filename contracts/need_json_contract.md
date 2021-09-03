### Request: get info on one need, identified by ID number 

```
{ need(id:28) 
  {
    title
    description  
    pointOfContact
    startTime 
    endTime 
    zipCode 
    supportersNeeded 
    status
    categories
      {
        id
        tag
      }
  }
}
```

### Successful response should look like

```
{
  "data": {
    "need": {
      "id": "28",
      "title": "Dicta aut quae.",
      "description": "Magni error eveniet. Rerum quisquam est. Sequi quo accusamus.",
      "pointOfContact": "breann@wisoky-doyle.co",
      "startTime": "2021-09-02 18:05:47 -0600",
      "endTime": "2021-09-02 18:05:48 -0600",
      "zipCode": "62677-9091",
      "supportersNeeded": 48,
      "status": "active",
      "categories": [
        {
          "id": "2",
          "tag": "Et."
        },
        {
          "id": "3",
          "tag": "Aut."
        }
      ]
    }
  }
}
```
