# Reading 14 Notes

[Home](README.md)

# Routing and Navigation Properties

## Routing in ASP.NET Core
### What is routing?
Routing is what matches incoming HTTP requests and executing those requests to the app's executable endpoints. Endpoints are the app's units of executable request-handling code. They are used in the app and configure when the app is started. The endpoint matching process can take values from the requested URL and provide the values for processing.Routing is able to be used to generate URLs that map to endpoints.
### Apps can configure routing by using:
- Controllers
- Razor Pages
- SignalR
- gRPC Services
- Endpoint-enabled middleware such as Health Checks
- Delegates and lambdas registered with routing

### Some Comparisons between terminal middleware and routing:
1. Both appraoches allow terminating the processing pipeline:
- Middleware gets rid of the pipeline by returning instead of invoking *next*.
- Endpoints are *always* terminal.
2. Terminal middleware allow positioning the middleware arbitrary place in the pipeline:
- Endpoints execute at the position of useendpoints.


### URL Matching
#### What is URL matching?
URL matching is the process of which routing matches an incoming request to endpoints.
This is based on data in path and headers of the URL.
Can be extended to consider any data in the request.