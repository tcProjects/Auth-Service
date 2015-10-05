* authenticate user request
  * GET
```json
{
	"username": "<name>",
	"password": "<password>"
}
```
* authenticate user response
```json
{
	"result": "user-authenticated",
	"token": "THISAUTHTOKEN"
}
```

* create user request
  * POST
```json
{
	"username": "<name>",
	"password": "<password>",
	"role": "<role>"
}
```
* create user response
```json
{
	"result": "user-created",
	"token": "THISAUTHTOKEN"
}
```

* delete user request
  * DELETE
```json
{
	"username": "<name>",
	"password": "<password>"
}
```
* delete user response
```json
{
	"result": "user-deleted"
}
```
