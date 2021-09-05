## Request
To: `https://barn-raiser-be.herokuapp.com/graphql`
Notes: 
* Need input should be the ID of an existing need
* Name, email, and need are all required fields

```
mutation {
  createSupporter(input:
		    {
		      name: "Aliya"
		      email: "supporter@example.com"
		      need: 1
		    }
  		)

		  {
		    supporter {
			  id
			  name
			  email
			  need
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
			    }
			}
		  errors
		}
}
```



## Succesful Response
```
{
  "data": {
    "createSupporter": {
      "supporter": {
        "id": "1",
        "name": "Aliya",
        "email": "supporter@example.com",
        "need": {
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
          ]
        }
      },
      "errors": []
    }
  }
}

```
