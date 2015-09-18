# Auth-Service
Simple service for administering users and providing authentication and authorization information


## Requirements

This service should enable the following use cases:

* a call can be made to check the complexity of a password and provide a strength score
* a user can be created with a username and password based on this service's minimum strength requirement
* a user can be created with an auto-generated apiKey and Secret
* a user's apiKey and Secret can only be retrieved by someone with that user's credentials
* a user can have personal information saved about them - i.e. address, email, name, etc. and this information is saved on an apikey basis
* a call exists to validate a user login and authenticate them
* a call exists to retrieve an encoded user context token, where the token is returned by the authentication call
* a user can have role/authorization information stored about them on an apikey basis
* all calls except user creation must be accompanied by an apikey and signed with the secret
* all responses except to retrieve the apikey and secret or create a user must be signed with the secret
