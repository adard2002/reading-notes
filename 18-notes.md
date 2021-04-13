# Reading 18 Notes

[Home](README.md)

# JWT Tokens and Claims

### Identity
Identity have 3 classes which are represented as the user: Claim, ClaimsIdentity, and ClaimsPrinciple
1. Claims: These represent a single fact about the user, i.e: first name, last name, age, etc. A single claim will only be a single piece of information. As an example a claim representing something about a user Bobby Bill could be his first name: Bobby and the second claim would be the last name being Bill. The most common constructor accepts two string which are type and value. While the type parameter is the name of the claim, the value is the info the claim is showing about the user.
2. ClaimsIdentity: This represents a form of identification or proving if the user is really the user. This is like someone trying to register into a login as you and there could be some varification questions that only you would know. 
3. ClaimsPrincipal: This represents the actual user. This means that the user can have one or more ways to claim their identity or prove its really them. This is pretty much like ClaimIdentity but can have more than one.

### Commands and behaviors
- Authenticate: Gets the user's information if there is any (decodes users cookie if any exist)
- Challenge: Requesting authentication or verification from the user or showing a login page
- SignIn: Persists the users information somewhere (writes cookies)
- SignOut: Removes users persisted information (deletes cookies)
- Forbid: Denies access to a resource like when trying to login to a site and you are denied access. 


