# JSON Web Tokens (JTW)


## Read
- [JWT Authentication in a React-Redux app (Scalac)](https://blog.scalac.io/react-redux-jwt-authentication.html)

## Example Projects
- https://github.com/StephenGrider/AdvancedReduxCode
- https://github.com/DimitriMikadze/node-redux-auth



# JWT Notes from 'The JWT Handbook'

## JWS - JSON Web Signature
- Signatures are useful to validate datta against tampering

## JWE - JSON Web Encryption
- Encryption is useful to protect data from being read by third parties

## Parts of JWT
- Header
- Payload
- Signature


## what

> An unsigned JWT should be considered invalid

> **2.1.1.2 Cross-Site Request Forgery (CSRF):**
> If JWTs (and session data) are not stored as cookies, CSRF attacks
are not possible.

> **2.1.1.3 Cross-Site Scripting (XSS):**
> Are still possible with JWT

## Architecture
### An application does not need to have only 1 JWT. For example, a shoppin application could have 3
- One JWT for the ID token, a token that carries the user’s profile information, useful for the
UI.
- One JWT for interacting with the API backend (the access token).
- One JWT for our client-side state: the shopping cart.

## Algorithms
The specification also defines a series of recommended algorithms:
- RSASSA PKCS1 v1.5 using SHA-256, called RS256 in the JWA spec.
- ECDSA using P-256 and SHA-256, called ES256 in the JWA spec.

*JWA is the JSON Web Algorithms spec, RFC 7518 2 .*