# HTTP
HyperText Transfer Protocol

we use http to communicate between machines over the web
it is a standardized way of communicating text over the web

when two machines communicate, they take on client and server role the client asks for resource from server, server provides it

## HTTP Request
Client requests for resources from a server
### Start Line
    - Method Verb: GET, PUT, POST, DELETE, OPTION
    - Target: Where? (URL)
### Request Body
    - Payload, especially for PUT and POST request
### Request Header
    - Information about the request itself

## HTTP Response
### Status Line
    - Status Codes
### Response Header
    - information about the response
### Response Body
    - Contains the resource client has asked for

## Status Codes
    - 1xx: Informational ('mmkay') 
    - 2xx: Success (We got the request, and we successfully fulfilled it)
    - 3xx: Redrection(we moved it)
    - 4xx: Client side error (you did something bad)
    - 5xx: Server side error (oops our fault)

    - 404: Resource Not Found
        - Do not use this to signal that there is no content to return
    - 204: NO Content
        - For when request successful but no information at request available
    - 503: Service Unavailable
    - 403: Forbidden

# RESTful API
REST: stands for REpresentational State Transfer
API: Application Programming Interface
    - An interface for machines/programs/applications

REST is a design guideline to build an API that is easy to understand and use

## SOA: Service Oriented Architecture
It's a more modularized way of designing your appliction - instead of your server solely existing for your UI app, we design the server to exist as a service that your UI can use, but also other machines can use. We build API's to share the data.

## REST Guiding Principles
    - Client - Server
        - it's a one way relationship
    - Stateless
        - the server should not be storing client's state
    - Cachable
        - Certain high demand server resources can be cached for quicker access
    - Uniform Interface
        - Your API should follow some kind of standardized way of accessing your resource
    - Layered System
        - Each layer in your server should only know the layer beyond
            - Dependency inversion and injection
    - Code on Demand (Optional)
        - Your server can also serve code snippets instead of text

# ASP.NET Core
ASP.NET Core is a Web Application framework for .NET Core that provides tools for building API's and applications

## Creating an API in C#
    - install the package `Swashbuckle.AspNetCore`
    - run the command `dotnet new web` in the terminal to create a new web application.
        - If you are using Visual Studio add a new ASP.NET WebApp that is EMPTY
    - add the connection string inside the appsetting.json/appsettings.Development.json (I had to do it in both when using Visual Studio 2022)
    - use the method `builder.Services.Add...` to add dependencies inside the API 
        - Either Singleton, Scoped, or Transient
    - add the method `builder.Services.AddEndpointsApiExplorer()`
    - add the method `builder.Services.AddSwaggerGen()`
