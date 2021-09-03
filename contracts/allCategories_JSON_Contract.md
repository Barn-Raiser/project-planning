### Request: 

To: `https://barn-raiser-be.herokuapp.com/graphql`

```
{ allCategories
  {
    id
    tag
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
            },
            {
                "id": "2",
                "tag": "Organizing / Event Management"
            },
            {
                "id": "3",
                "tag": "Delivery"
            },
            {
                "id": "4",
                "tag": "Handiwork"
            },
            {
                "id": "5",
                "tag": "Transportation"
            },
            {
                "id": "6",
                "tag": "Food Prep"
            }
        ]
    }
}
```
