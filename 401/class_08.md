# Code 401 Class 08 Reading Notes

## When is Basic Authorization used vs. Bearer Authorization
* Basic authorization is used for initial sign in to verify a users authenticity. Once authentication is complete than a user is issued a token and from then on bearer authorization is used to verify cthat a user has been authenticated.

## What does the JSON Web Token package do
* The json web token pagackage or jwt allows javascript developers the ability to create/sign json web tokens and to verify them. It is a package that allows for server side bearer authorization

## What considerations should we make when creating and storing a SECRET
* The SECRET is what verifiesa jwt /anonymizes a jwt and therefore it is incredibly important to keep obfuscated when it comes to bearer authorization. A good way to achieve this is storing the SECRET in the .env file so that it is always only on the server side

## Define the following terms
* Encryption
  * Encryption is the proccess of transforming data into another form that requires a cipher to decode. One npm package that can be used for this is bcrypt.
* Token
  * A token is a piece of data that is usually given to a user in exchange for an authorization code after basic authorization. This token allows for a user to pass bearer authorization
* Bearer
  * A bearer is a user that has gone through basic authorization and has a token as a result. The token allows the bearer access to certain routes and information from a server
* Secret
  * A secret in the form of a web token is a value that is added to a token as part of the signature and this allows servers/clients to be able to verify that a token has not been modified.
* JSON Web Token
  * A JSON web token is a form of token that can be used for bearer authorization. A jwt consists of a header, payload, and secret that is encoded in a special format. The secret is used as part of the signature which allows a server to verify that the token has not been modified.


[Table of Contents](README.md)