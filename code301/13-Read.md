# Reading 13 Notes

[Home](README.md)
## Sending Form Data
### How to send the data
The form element defines how the data will be sent to the page. The 2 most important attributes to the form tag are the action and method. The action attribute tells you where the data gets sent. This attribute will likely have a url after it. The method attribute tells you how the data is sent. There are a couple different types of methods:
1. GET method: Asks the browser to return and send back a given source. 
2. POST method: This is a little bit different than the GET method. This method looks at the data that was given and sends back a result.
### HTTP requests
HTTP requests are never displayed to the user. If you want to use a password or something that is kind of like a spoiler do NOT use the GET request. Because with this you will risk exposing the text in the URL bar. This is why it is recommended to use a POST request because this way it will not show in the URL at the top of the page in the search bar.
If you want to send a large amount of info or data it is recommended that you use the POST method. This is because the POST method limits the amount or length of the URL being shown and displayed to the page.

## HTML5 Forms Reference https://htmlreference.io/forms/ 
Action and method attributes used in a form element in the HTML. 
1. action: Indicates which URL the form's info is sent to once submitted
- There are 2 different ways you can do this. with either a relative URL which is inside of the file or repository you are editing (Example: "/contact). Or you can use an absolute URL which is a link taken from your browser. (Example: "https://htmlreference.io/contact").
2. method: Indicates the HTTP method used when submitting the form.
- There are 2 different ways you can do this. Either "post" or "get". Post allows the form information to be sent to server as part of the request body. The get attribute makes it so the information is sent to he server as a part of URL parameters.

## https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK 