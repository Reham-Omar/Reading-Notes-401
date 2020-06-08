# Bearer Authorization

## Bearer Token

- “Bearer Token”: secondary authentication method .
- Bearer Tokens are encoded JSON objects that “bear” or “contain” enough information for the server to assert that any client request that presents a valid token must have originated from a client that has previously authenticated themselves using either Basic or OAuth. Upon receiving a Bearer Token from a client, the server can decode it, inspect the JSON object inside, look up the appropriate account, and re-authenticate the user in a single lookup.

- Bearer Tokens are sent to the user/client after the initial `signin` process has completed.
- Clients must make every subsequent request to the server with that token, in the header
- `Authorization: Bearer encoded.jsonwebtoken.here`
- The server opens the token, does the re-authentication, and then grants or denies access
- In express servers, this can be done in middleware, in conjunction with a user model

## JSON Web Tokens

- JSON Web Token (JWT) is an open standard that defines a compact and self-contained way for securely transmitting information between parties (servers, clients, etc) as a JSON object.
- This information can be verified and trusted because it is digitally signed.
- Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens.
- Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties.
- When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

## When should you use JSON Web Tokens?

- Authorization
- Information Exchange

![Image](img/bearer.png)
