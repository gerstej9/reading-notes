# Code 401 Class 07 Reading Notes


## Write the following JWT steps in the correct order
1. Register your application to get a client_id and client_secret
1. Ask the client if they want to sign in via a third party
1. Redirect to a third party authentication end point
1. Make a request to third-party API endpoint
1. Receive authorization code
1. Make a request to the access token endpoint
1. Receive access token

## What can you do with an authorization code
* An authorization code allows you to exchange the code for an access token in return
* [Source oauth](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/#:~:text=The%20authorization%20code%20is%20a,approve%20or%20deny%20the%20request.)

## What can you do with an access token?
* Access tokens are what applications use to make requests on behalf of the cline, it is a representation of authorization.
* [Source oauth](https://www.oauth.com/oauth2-servers/access-tokens/#:~:text=Access%20tokens%20are%20the%20thing,in%20transit%20and%20in%20storage.)

## What is the benefit of using OAuth instead of your own basic authentication?
* Oauth does not share passwords but instead uses authorization tokens. It allows you to approve an application interaction on your behalf without the need for a password
* [Source Varonis](https://www.varonis.com/blog/what-is-oauth/#:~:text=OAuth%20doesn't%20share%20password,without%20giving%20away%20your%20password.)

## Define the following terms
* Client ID
  * A client id is an identifier for your app and is received upon registration
* Client Secret
  * Client secret is a special string that is concatenated onto tokens which acts as part of the signature for a token to ensure they have not been modified
* Authentication Endpoint
  * An authentication endpoint is where a client is sent initially for them to input username and password or other credentials to become authorized and receive and authorization code
* Access Token Endpoint
  * The access token endpoint is where the user goes after receiving an authentication code and in exchange for their code they receive an access token.
* API endpoint
  * Once the user has an access token they have a "passport" to access the various api endpoints that are associated with the app or their personal account
* Authentication Code
  * An authentication code is what is given to a user after they have inputed credentials and been authorized by a third party. This is used to prevent an app needing to interact directly with a user's password
* Access Token
  * Access tokens are given in exchange for an authentication code once a user has been authorized. It indicates to an app that the user can interact with the app. Access tokens in the form of JSON Web Tokens (JWT)s have a header, payload, and a signature. The signature is composed of the header, payload, and a secret and this allows for proof of signature and a way to look for modifications/tampering. Access tokens are not meant to hold secure information as much as they are meant to be used once a user is already authorized.


[Table of Contents](README.md)