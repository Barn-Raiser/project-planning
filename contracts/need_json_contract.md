### Request: 

To: `https://barn-raiser-be.herokuapp.com/graphql`    
Returns data for a single need

```
{ need(id:6) 
  {
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
      {
        id
        tag
      }
    supporters{
      id
      name
      email
    }
  }
}
```

### Successful response

```
{
  "data": {
    "need": {
      "id": "6",
      "title": "Let's clean up the park!",
      "description": "There's lots of litter in the park - let's clean it up.",
      "pointOfContact": "aliya@test.com",
      "startTime": "2021-09-30 11:00",
      "endTime": "2021-09-30 3:00",
      "zipCode": "80218",
      "supportersNeeded": 12,
      "status": "active",
      "categories": [
        {
          "id": "1",
          "tag": "Fuga."
        },
        {
          "id": "3",
          "tag": "Sunt."
        }
      ],
      "supporters": [
        {
          "id": "5",
          "name": "Tanner",
          "email": "supporterTNR@example.com"
        },
        {
          "id": "6",
          "name": "Aliya",
          "email": "aliya_supporter@example.com"
        }
      ]
    }
  }
}
```
