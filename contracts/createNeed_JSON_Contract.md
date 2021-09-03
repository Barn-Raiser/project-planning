# Phase 1
## Request 
* NOTE: Category ID(s) must match the IDs of categories in the DB, which can be retrieved with the [allCategories query](https://github.com/Barn-Raiser/project-planning/blob/main/contracts/allCategories_JSON_Contract.md) 
```
mutation {
  createNeed(input:
	     {
	      pointOfContact: "aliya@test.com"
	      title: "Let's clean up Cheesman park!"
	      description: "There's lots of litter in the park - let's clean it up."
	      startTime: "9/30/2021 11:00AM"
	      endTime: "9/30/2021 3:00PM"
	      streetAddress: "Cheesman Park"
	      city: "Denver"
	      state: "CO"
	      zipCode: "80218"
	      supportersNeeded: 12
	      categories: [2, 4]
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
	    {
              id
              tag
            }
        }
  errors
	}
}
```

## Response (with requested data returned)
```{
    "data": {
        "createNeed": {
            "need": {
                "id": "2",
                "title": "Let's clean up Cheesman park!",
                "description": "There's lots of litter in the park - let's clean it up.",
                "pointOfContact": "aliya@test.com",
                "startTime": "9/30/2021 11:00AM",
                "endTime": "9/30/2021 3:00PM",
                "zipCode": "80218",
                "supportersNeeded": 12,
                "status": "active",
                "categories": [
                    {
                        "id": "2",
                        "tag": "Organizing / Event Management"
                    },
                    {
                        "id": "4",
                        "tag": "Handiwork"
                    }
                ]
            },
            "errors": []
        }
    }
}
```
