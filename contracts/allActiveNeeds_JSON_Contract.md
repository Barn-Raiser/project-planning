### Request: 

```
{ allActiveNeeds 
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
    categories{
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
    
### Sample Successful Response: 
```
{
  "data": {
    "allActiveNeeds": [
      {
        "id": "1",
        "title": "Qui maiores suscipit.",
        "description": "Illum quisquam rerum. Atque reiciendis explicabo. Incidunt ducimus est.",
        "pointOfContact": "fiona.macgyver@botsford-frami.io",
        "startTime": "2021-09-05 11:09:10 -0600",
        "endTime": "2021-09-05 11:09:11 -0600",
        "zipCode": "35233-1863",
        "supportersNeeded": 22,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Fuga."
          },
          {
            "id": "2",
            "tag": "Corporis."
          },
          {
            "id": "3",
            "tag": "Sunt."
          }
        ],
        "supporters": [
          {
            "id": "1",
            "name": "Aliya",
            "email": "supporter@example.com"
          },
          {
            "id": "2",
            "name": "Tanner",
            "email": "supporterTNR@example.com"
          }
        ]
      },
      {
        "id": "2",
        "title": "Adipisci necessitatibus deleniti.",
        "description": "Vel fuga ullam. Culpa neque commodi. Dicta voluptas illo.",
        "pointOfContact": "stewart@towne-hansen.biz",
        "startTime": "2021-09-05 11:09:10 -0600",
        "endTime": "2021-09-05 11:09:11 -0600",
        "zipCode": "85413",
        "supportersNeeded": 70,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Fuga."
          }
        ],
        "supporters": [
          {
            "id": "3",
            "name": "Tanner",
            "email": "supporterTNR@example.com"
          }
        ]
      },
      {
        "id": "3",
        "title": "Molestiae accusantium ad.",
        "description": "Officiis ea magni. Quia ut non. Est explicabo nam.",
        "pointOfContact": "kara@haley.org",
        "startTime": "2021-09-05 11:09:10 -0600",
        "endTime": "2021-09-05 11:09:11 -0600",
        "zipCode": "24733",
        "supportersNeeded": 14,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Fuga."
          }
        ],
        "supporters": [
          {
            "id": "4",
            "name": "Tanner",
            "email": "supporterTNR@example.com"
          }
        ]
      },
      {
        "id": "4",
        "title": "Doloribus quis nesciunt.",
        "description": "Nam totam aliquam. Sapiente omnis deleniti. Est eaque quas.",
        "pointOfContact": "dewey@cronin-muller.info",
        "startTime": "2021-09-05 11:09:10 -0600",
        "endTime": "2021-09-05 11:09:11 -0600",
        "zipCode": "06976",
        "supportersNeeded": 20,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Fuga."
          }
        ],
        "supporters": []
      },
      {
        "id": "5",
        "title": "Autem omnis qui.",
        "description": "Dolor distinctio incidunt. Inventore dolorem eius. Repellendus ipsam laborum.",
        "pointOfContact": "marta@cormier.io",
        "startTime": "2021-09-05 11:09:10 -0600",
        "endTime": "2021-09-05 11:09:11 -0600",
        "zipCode": "39410",
        "supportersNeeded": 71,
        "status": "active",
        "categories": [
          {
            "id": "2",
            "tag": "Corporis."
          },
          {
            "id": "3",
            "tag": "Sunt."
          }
        ],
        "supporters": []
      },
      {
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
    ]
  }
}
```
