### Request: 

```
{ allActiveNeeds 
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
    
### Sample Successful Response: 
```{
  "data": {
    "allActiveNeeds": [
      {
        "id": "24",
        "title": "Dolore reprehenderit adipisci.",
        "description": "Incidunt corrupti autem. Ut temporibus sit. Eos est aut.",
        "pointOfContact": "laveta@pollich.biz",
        "startTime": "2021-09-02 18:05:47 -0600",
        "endTime": "2021-09-02 18:05:48 -0600",
        "zipCode": "12484-3107",
        "supportersNeeded": 96,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Saepe."
          },
          {
            "id": "2",
            "tag": "Et."
          },
          {
            "id": "3",
            "tag": "Aut."
          }
        ]
      },
      {
        "id": "25",
        "title": "Totam vel eligendi.",
        "description": "Occaecati eum tempore. Quisquam omnis quia. Enim labore dolorem.",
        "pointOfContact": "danial@wunsch.co",
        "startTime": "2021-09-02 18:05:47 -0600",
        "endTime": "2021-09-02 18:05:48 -0600",
        "zipCode": "66570",
        "supportersNeeded": 17,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Saepe."
          }
        ]
      },
      {
        "id": "26",
        "title": "Adipisci rerum fugiat.",
        "description": "Excepturi quis autem. Perferendis distinctio modi. Sit nihil esse.",
        "pointOfContact": "kara_hand@yost.net",
        "startTime": "2021-09-02 18:05:47 -0600",
        "endTime": "2021-09-02 18:05:48 -0600",
        "zipCode": "98980-6965",
        "supportersNeeded": 97,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Saepe."
          }
        ]
      },
      {
        "id": "27",
        "title": "Soluta ut quasi.",
        "description": "Ipsam tempora est. Et quod facere. Atque tempore dicta.",
        "pointOfContact": "clement_harvey@heathcote.biz",
        "startTime": "2021-09-02 18:05:47 -0600",
        "endTime": "2021-09-02 18:05:48 -0600",
        "zipCode": "93501-9150",
        "supportersNeeded": 57,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Saepe."
          }
        ]
      },
      {
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
      },
      {
        "id": "29",
        "title": "This is a new need",
        "description": "More about my new need",
        "pointOfContact": "aliya@test.com",
        "startTime": "string value",
        "endTime": "string value",
        "zipCode": "string value",
        "supportersNeeded": 12,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Saepe."
          },
          {
            "id": "3",
            "tag": "Aut."
          }
        ]
      },
      {
        "id": "30",
        "title": "Let's clean up the park!",
        "description": "There's lots of litter in the park - let's clean it up.",
        "pointOfContact": "aliya@test.com",
        "startTime": "9/30/2021 11:00AM",
        "endTime": "9/30/2021 3:00PM",
        "zipCode": "80218",
        "supportersNeeded": 12,
        "status": "active",
        "categories": [
          {
            "id": "1",
            "tag": "Saepe."
          },
          {
            "id": "3",
            "tag": "Aut."
          }
        ]
      }
    ]
  }
}
```
