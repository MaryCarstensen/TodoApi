use Postman to test this (evidently todo is not case sensitive as Todo also works)
first start debugging and note where the local host is, debugging must be running as the memory for this project is local!
GET to http://localhost:59310/api/todo (substitute the local host in), this should return all the "Todo items"
POST to http://localhost:59310/api/Todo with body, raw, json { "name": "itemName", "isComplete":false}, this should create a new item in the Todo item collection and returns a 201 Created and the item
PUT to http://localhost:59310/api/Todo/1 with body, raw, json { "id": 1, "name": "newName", "isComplete": true}, this should update item 1 and returns a 204 No Content response
DELETE to http://localhost:59310/api/Todo/2 this will delete item 2 and returns a 204 No Content response
