# Web API Desiging Rules

## Design

Use [Swagger 2.0](http://swagger.io/) to design / define API. And provide JSON/YAML format document for it. You can use [Swagger Editor](editor.swagger.io) to design APIs.

## Versioning

Use [Semantic versioning](http://semver.org/). Major version will be changed when you need to do braking changes. Minor/Patch version up might keep backward compatibility.

Include version number in URL like `http://api.example.com/v1/users`. use "v" + major version. Never include minor version because minor version up need to ensure backward compatibility.

## URL and HTTP Methods

You should consider URL as "nouns" and HTTP Methods as "verbs". Means if you need to create the API to get users, it should be `GET /users`. Not `POST /users/get_list`.

## URL must be case insensitive

You should only use small letters. Never do `/api/v1/me/userRoles`. use `/api/v1/me/user-roles`.
And you should use spinal case ( Hyphen separated case ) such as "user-roles" on URLs. Don't use snake case ( user_roles ). It's for consistency.

## Use proper status code for response

200 means ok. 404 means not found. and 201 means "created". 401 means unauthorized. You should return proper status code and define what kind of status code will be returned on the document.

## Never use envelope response data structure

Envelope means the following common structure of response data.

```json
{
	"header" : {
		"statusCode": 200,
		"status": "ok",
	},
	"body": {
		"users" : [
			...
		],
	}
}
```

Never design this kind of structure because HTTP response itself is already envelope and you can add additional header info to HTTP Response header.
