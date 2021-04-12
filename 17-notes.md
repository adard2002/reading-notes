# Reading 17 Notes

[Home](README.md)

# Intro to Identity

## HTTP Cookies
A web cookie or browser cookie is a small piece of data that a server sends to the user's web browser. The browser can store it and send it back later when that specific data is requested to the same server. This is usually used to tell if 2 requests came from the same browser like keeping a user logged-in. The 3 main uses or purposes for HTTP Cookies are:<Br>
1. Session management: This is like logins or the shopping cart you would have on amazon or some store online. This is used for anything the server should remember<br>
2. Personization: Preferences on your profile for example. And themes or other profile settings.<Br>
3. Tracking: Recording user behavior or keeping in mind where the user has gone.

## Defining lifetime of a cookie
- Session: These cookies are deleted when the current session ends. This is like if you end your browser it will disappear and will have to do whatever you were doing over again<br>
- Permanent: These cookies are deleted at a specified date by the Expires attribute or the Max-Age attribute.

## Different attributes and their uses
Cookies can be defined on where to be sent by using the Domain and Path attributes to define the scope of the cookies or what URLs the cookies should be sent to.
- Domain: Specifies which hosts are allowed to receive the cookie. 
- Path: tells you that a URL path must exist in the requested URL in order to actually be able to send the Cookies header. 

## Cookie Prefixes
__Host- : When this is the prefix a cookie name has it means it is accepted in a Set-Cookie header only if it's also marked with the Secure attribute<Br>
__Secure- : When this is the prefix a cookie name has it means it's accepted in a Set-Cookie header only if it's marked with the Secure attribute and is sent from a secure origin.

## Security
Ways to avoid attacks involving cookies:
- Use the HttpOnly attribute to prevent access to cookies values using JavaScript
- With sites with personal or sensitive information should have a short lifetime and should use the SameSite attribute set to Strict or Lax. Strict is when the cookie is sent only to the same site as it was originated. While lax, excepts that cookies are sent when the user navigates to the cookie's origin site.