# Auth-Service
Simple service for administering users and providing authentication and authorization information


## Requirements

Make a store for apiKey and Secret storage which is managed outside of this service.  Maybe in an apiKey service?

This service should enable the following use cases:

* a call can be made to check the complexity of a password and provide a strength score
* a user can be created with a username and password based on this service's minimum strength requirement
* a user can have personal information saved about them - i.e. address, email, name, etc. and this information is saved on an apikey basis
* a call exists to validate a user login and authenticate them takes apiKey to associate to token, returns a token good for 15 minutes to access user info
* a user can have role/authorization information stored about them on an apikey basis
* all calls must be accompanied by an apikey and signed with the secret
* all responses must be signed with the secret
