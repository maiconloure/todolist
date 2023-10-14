# TODO - JAVA - API

Technologies: Java, Maven, SpringBoot, Lombok, Jpa

## Available routes

### New User
> **POST** /users
```json
{
  "username": "Test",
  "name": "Test",
  "password": "123"
}
```

### Get User Tasks
Method: GET <br/>
Path: /tasks <br/>
Authorization: Basic Auth <br/>
```json
[
	{
		"id": "45efed89-caca-4cd7-8b0f-c0e50b19519a",
		"description": "An App for TODO List",
		"title": "ToDo List",
		"endAt": "2023-10-17T16:16:00",
		"priority": "HIGH",
		"createdAt": "2023-10-14T16:47:18.135405",
		"userId": "1ef77ada-d73a-48ed-960f-441f3d26b586",
		"startAt": "2023-10-16T16:14:00"
	}
]
```
### New Task
Method: POST <br/>
Path: /tasks <br/>
Authorization: Basic Auth <br/>
```json
{
	"title": "To Do List",
	"description": "An App for TODO List",
	"priority": "HIGH",
	"startAt": "2023-10-16T16:14:00",
	"endAt": "2023-10-17T16:16:00"
}
```

### Update Task
Method: PATCH <br/>
Path: /tasks <br/>
Authorization: Basic Auth <br/>
```json
{
	"title": "New Title"
}
```
