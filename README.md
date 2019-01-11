# Go Learn Path

This repository should guide you the way from the installation of Go till advanced topics like memory management and Go routine scheduler and provide you links to public material.

## Overview

**Self-Study Learn Program**  
**Duration:** 4 Week  
**Q/A:** every Wednesday and Sunday  

**Course-Requirements**:
* basic CS knowledge
* practical experience with one serious language
* self-motivated
* considering to make Go your profession

**Course-Topics**:
1. Week: start with the basics
2. Week: microservice with gokit
3. Week: managing SQL entities
4. Week: publish/subscribe to message queue

**Tools and Platforms**:
* [Google Hangouts](https://hangouts.google.com/) or [Skype](skype.com) (for the Q/As)
* [github.com](github.com) account
* [go:latest](https://golang.org/dl/)
* [docker:latest](https://docs.docker.com/)
* [MS Visual Studio Code:latest](https://code.visualstudio.com/) with Extensions:
  * [Go](https://marketplace.visualstudio.com/items?itemName=ms-vscode.Go),
  * [Docker](https://marketplace.visualstudio.com/items?itemName=PeterJausovec.vscode-docker),
  * [VS Live Share Plugin](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)

## 1. Week: Start with the Basics

**Goal:** 
* to be able to read and write go code
* understand concepts/ideas and best practices of go
* to write and run unit, integration, benchmark tests

**Path:**
lets start with [https://golang.org/](https://golang.org/) and learn the basics.  
a must have here are 
* [Getting Started](https://golang.org/doc/install)
* [A Tour of Go](https://tour.golang.org/welcome/1)
* [How to write Go code](https://golang.org/doc/code.html)
* [Editor plugins and IDEs](https://golang.org/doc/editors.html)
* [Effective Go](https://golang.org/doc/effective_go.html)

Understand the core ideas behind Go from one of the creator's
* [dotGo 2015 - Rob Pike - Simplicity is Complicated](https://www.youtube.com/watch?v=rFejpH_tAHM)
* [Go Proverbs - Rob Pike - Gopherfest - November 18, 2015](https://www.youtube.com/watch?v=PAAkCSZUG1c)
* [Rob Pike - 'Concurrency Is Not Parallelism'](https://www.youtube.com/watch?v=cN_DpYBzKso)

Now that you know the basics about Go, it is time to get your hands dirty by writing simple algorithm. Pick some challenge from [https://www.reddit.com/r/dailyprogrammer/](https://www.reddit.com/r/dailyprogrammer/) and write Go. Focus on Test Driven Development using the standard Go testing package [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).

You should now be able to write unit test cases, simple function, structs and got familiar with Go Idiomatic.

### (Optional) Exercise 1.1: REST API & Client

Go has a powerful standard library, so let's go and check out the [net/http/](https://golang.org/pkg/net/http/) package.
Build a REST API & Client using the standard library only and write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/) and [https://golang.org/pkg/net/http/httptest/](https://golang.org/pkg/net/http/httptest/).

### (Optional) Exercise 1.2: Web App

Go also has a powerful template engine used not only for Web Apps but also in projects like [helm](https://helm.sh/) and [hugo](https://gohugo.io/). Build a simple Web App or Latex CV generator with [html/template/](https://golang.org/pkg/html/template/). Write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).

## 2. Week: Microservice with gokit

Gokit is a toolkit to create microservices with onion-like-layers: logging, instrumentation, transport, endpoints are layers that wraps the domain service. Therefore it allows developers to easily switch from REST/JSON API to a grpc/protobuf API by adding/replacing transportation layer and keep the service layer untouched.

A nice teaser to this toolkit is the talk from the creator [Golang UK Conference 2016 - Peter Bourgon - Go + Microservices = Go Kit](https://www.youtube.com/watch?v=JXEjAwNWays)

Read more about 
* [go-kit FAQ](https://gokit.io/faq/)
* [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)

A good starting point for the exercise are the examples in the repo [https://github.com/go-kit/kit](https://github.com/go-kit/kit)

### Exercise 2.1: Build REST/JSON API using go-kit

Choose a domain you know and build a REST/JSON API and REST client. Use the example in [https://github.com/go-kit/kit](https://github.com/go-kit/kit) as a guidline. Implement an InMemoryDatabase (we will replace it later on with a real one). Write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).

### (Optional) Exercise 2.2: Add grpc/protobuf transportation layer

Implement another transportation layer usign [grpc](https://grpc.io/) and [protobuf](https://developers.google.com). Write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).

## 3. Week: Managing entities with sql

Start with reading about [go-database-sql.org](http://go-database-sql.org/), [docs.docker.com/](https://docs.docker.com/) and how to run the \<database of your choice\> in docker. Read and try out [flywaydb.org/](https://flywaydb.org/) to create version controlled database schemas.
 
 ### Exercise 3.1: Build a database layer and manage your domain entities
 
 Implement a basic CRUD database layer using the \<database of your choice\>  running in docker. Write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).
 
 
### (Optional) Exercise 3.2: Implement Stress Benchmark Tests

Implement a benchmark test suite and measure your performance bottle necks. How much operation can your service process using a specific hardware setup ?

## 4. Week: Publish/Subscribe on a message queue

TBD

# Where to go from here on

Recommendations - for advanced Gophers:
* [Concurrency in Go](http://shop.oreilly.com/product/0636920046189.do)
* [Ultimate Go Programming, Second Edition](https://learning.oreilly.com/library/view/ultimate-go-programming/9780135261651/)  

Read Blogs/Books/Video  
Write Go idiomatic code  
Write a blog about go    
Hold a talk about go    
