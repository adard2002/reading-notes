# Reading 19 Notes

[Home](README.md)

# Roles, Claims and JWT Tokens

## Difference between Authentication and Authorisation
- Authentication: This is the process of determining *who you are*
- Authorisation: This is the process of determining *what you are allowed to do* this would be like permissions


## What is a JWT?
JWT stands for JSON Web Token; this means representing claims being transferred between two parties. This is a way of encoding JSON objects and using that encoded object as access tokens for authentication.

## Different parts that will be seen in JWTs
### 1- HEADER
```
{
 "alg": "HS256",
 "typ": "JWT"
}
```
- alg: This is used by 2 of the main algorithms (HS256/RS256), these are used to sign the JWT signature which will be mentioned in the headers so that the producer and consumer use the same algorithm to verify the token on either end.
- typ: Defines the typ of the token which is JWT in this case.

### 2- PAYLOAD
This contains the custom data along with some standard claims too. 
```
{
 "email": "John Doe",
 "xyz": "abc"
}
```
#### Some standard claims:
- Issuer (iss) - Tells you the principal(s) that issued in the JWT.
- Subject (sub) - Tells you the subject of the JWT.
- Audience (aud) - This claim identifies the recipients the JWT is intended for. Every principle is required to identify itself with a value in the audience claim.
- Experation time (exp) - This claim identifies the expiration time on or after the JWT must not be accepted for processing. 
- Not before (nbf) - This claim identifies the time on the JWT will start to be accepted for processing.
- Issued at (iat) - This claim identifies the time that the JWT was issued. 
- JWT ID (jti) - this is case sensitive and is a unique identifier of the token among different issuers.

### 3- SIGNATURE
This is calculated by the base64url encoding of the header and payload and concatenating them with a period as a separator.
```
key           = 'secretkey';
unsignedToken = encodeBase64Url(header) + '.' + encodeBase64Url(payload);
signature     = HMAC-SHA256(key, unsignedToken) // As mentioned in header section.
```
