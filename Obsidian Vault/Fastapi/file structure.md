backend
- core
	- dependencies package - contains functions and init
	- logger file - contains config file
	- security
		- providers -
			- auth provider - get access token, create access token, try get user
			- credential provider - authenticate, verify passwrord
			- Authentication provider that authenticats a user against an LDAP server using username/password combination
			- Authentication provider that authenticates a user using a token from OIDC ID token
		- hasher
		- security
	- setting
		- db provider
		- directories
		- settings
	- config - 
	- exceptions
	- relaease checker
	- root logger
- db
	- fixes
	- models
- lang
- route
	- contains the routes for different modules
- schema
	- conatins the basemodel schema for different modules
- scripts
- 