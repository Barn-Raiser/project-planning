### Request: 

To: `https://barn-raiser-be.herokuapp.com/graphql`   
Returns all categories in the database

```
{ allCategories
  {
    id
    tag
    supporters {
        name
        email
      }
  }
}
```
    
### Successful Response: 
```

{
    "data": {
        "allCategories": [
            {
                "id": "1",
                "tag": "Other"
                "supporters": [
                  {
                    name: "albert"
                    email: "testing@test.com", 
                  }, 
                  {
                    name: "bob"
                    email: "bobifier@test.com", 
                  }
                ]
            },
            {
                "id": "2",
                "tag": "Organizing / Event Management"
                "supporters": [
                  {
                    name: "albert"
                    email: "testing@test.com", 
                  }, 
                  {
                    name: "rob"
                    email: "robifier@test.com", 
                  }
                ]
            },
            {
                "id": "3",
                "tag": "Delivery"
                "supporters": [
                ]
            },
            {
                "id": "4",
                "tag": "Handiwork"
                "supporters": [
                  {
                    name: "kat"
                    email: "kitty@test.com", 
                  }, 
                  {
                    name: "rob"
                    email: "robifier@test.com", 
                  }
                ]
            },
            {
                "id": "5",
                "tag": "Transportation"
                "supporters": [
                  {
                    name: "trucker"
                    email: "driver@test.com", 
                  }
                ]
            },
            {
                "id": "6",
                "tag": "Food Prep"
                "supporters": [
                  {
                    name: "pupper"
                    email: "kitty@test.com", 
                  }
                ]
            }
        ]
    }
}
```
