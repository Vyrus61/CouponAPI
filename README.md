# CouponAPI

Brief project description and purpose.

## Table of Contents

- [API Overview](#api-overview)
  - [API Architecture](#api-architecture)
  - [REST APIs](#rest-apis)
    - [Key Features](#key-features-of-rest-apis)
  - [Web API](#web-api)
  - [Minimal API](#minimal-api)
    - [Key Features](#key-features-of-minimal-api)
      - [Request Object](#request-object)
      - [Response Object](#response-object)
      - [Headers and Content](#headers-and-content)
- [Libraries Used](#libraries-used)
  - [AutoMapper](#automapper)
  - [FluentValidation](#fluentvalidation)
  - [EntityFrameworkCore](#entityframeworkcore)
    - [Basic DbContext](#basic-dbcontext)
- [Getting Started](#getting-started)

## API Overview

APIs are mechanisms that enable two software components to communicate with each other using a set of definitions and protocols.

### API Architecture

API architecture is typically explained in terms of client and server. The application sending the request is called the client, and the application sending the response is called the server.

#### SOAP APIs

These APIs use Simple Object Access Protocol. Client and server exchange messages using XML. This is a less flexible API that was more popular in the past.

#### RPC APIs

These APIs are called Remote Procedure Calls. The client completes a function (or procedure) on the server, and the server sends the output back to the client.

#### Websocket APIs

Websocket API is another modern web API development that uses JSON objects to pass data. A WebSocket API supports two-way communication between client apps and the server. The server can send callback messages to connected clients, making it more efficient than REST API.

#### REST APIs

These are the most popular and flexible APIs found on the web today. The client sends requests to the server as data. The server uses this client input to start internal functions and returns output data back to the client. Let’s look at REST APIs in more detail below.

REST stands for Representational State Transfer. REST defines a set of functions like GET, PUT, DELETE, etc. that clients can use to access server data. Clients and servers exchange data using HTTP.

#### Key Features of REST APIs

- **Statelessness:** Servers do not save client data between requests.
- **Standard Functions:** Defined set of functions (GET, PUT, DELETE, etc.) that clients use to interact with the server.
- **HTTP Communication:** Data exchange between clients and servers is done using HTTP.

### Web API

A Web API or Web Service API is an application processing interface between a web server and web browser. All web services are APIs but not all APIs are web services. REST API is a special type of Web API that uses the standard architectural style explained above.

### Minimal API

It is a web API but it is the simplified version of it without a controller that .Net uses in the Web API project.

#### Key Features of Minimal API

- **No Controllers:** Minimal API doesn't require the use of controllers.
- **Route Params:** Basic GET and POST endpoints without using `add.Controller`.
- **Simplified Routing:** Very simple to add route parameters.

##### Request Object

Request Object information goes here...

##### Response Object

Response Object information goes here...

##### Headers and Content

Headers and Content information goes here...

## Libraries Used

### AutoMapper

AutoMapper is a simple little library built to solve a deceptively complex problem - getting rid of code that mapped one object to another.

### FluentValidation

FluentValidation is a .NET library for building strongly-typed validation rules.

### EntityFrameworkCore

EntityFrameworkCore is a library for database connection and more.

#### Basic DbContext

Basic DbContext information goes here...

## Getting Started

1. In the `Program.cs`, add the necessary dependencies.
2. Run the following commands to add migration and update the database:

```bash
dotnet ef migrations add AddCouponToDb
dotnet ef database update
