# API_Dev
---
creating a restful api

### Chapter One
Restful API

HTTP Methods
GET
POST
PUT
UPDATE
DELETE
---
We are going to build an API that lists all the recipes stored in our system. The API will be designed to return different results with different URLs. For example, http://localhost:5000/recipes is going to give us all the recipes stored in our system, while http://localhost:5000/recipes/20 will give us the recipe with ID = 20. Upon successful recipe retrieval, we will also see the HTTP status is set to 200 (OK). This indicates that our request has been successful.

When we create a new recipe, we use the HTTP POST method to query http://localhost:5000/recipes with all the necessary parameters to describe our recipe in JSON format. The JSON format is simply a key/value pair. If our request is successful, the recipe will be created in the backend and will return HTTP status 201 (Created). Together with the HTTP status, it will also send the recipe that has just been created in JSON format.

When we update a recipe, we use the HTTP PUT method to send the data to http://localhost:5000/recipes/20 with all the necessary parameters for the updated recipe in JSON format. If our request is successful, the recipe will be updated in the backend and it will return HTTP status 200 (OK). Together with the HTTP status, it will also send the updated recipe in JSON format.

When we delete a recipe, we can use the HTTP Delete method to send the data to http://localhost:5000/recipes/20. This will remove the recipe with ID = 20.

Now you know where we are heading to, let's roll up our sleeves and get our hands dirty!
