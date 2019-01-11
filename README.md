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

### (Optional) Exercise 1: REST API & Client

Go has a powerful standard library, so let's go and check out the [net/http/](https://golang.org/pkg/net/http/) package.
Build a REST API & Client and write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).

### (Optional) Exercise 2: Web App

Go also has a powerful template engine used not only for Web Apps but also in projects like [helm](https://helm.sh/).  
Build a simple Web App with [html/template/](https://golang.org/pkg/html/template/).

## Go kit

Go kit is a toolkit to create microservices with onion-like-layers, logging, instrumentation, transport, endpoints.
Therefore it allows the developers to easily switch from REST JSON API to a grpc protobuf API by replacing layers and keep the service layer untouched.

A nice teaser to this toolkit is the talk from the creator [Go + Microservices = Go Kit [I] - Peter Bourgon, Go Kit](https://www.youtube.com/watch?v=NX0sHF8ZZgw)

Read more about 
* [go-kit FAQ](https://gokit.io/faq/)
* [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)

A good starting point for the exercise are the examples in the repo [https://github.com/go-kit/kit](https://github.com/go-kit/kit)

### Exercise 3: Build REST API using go-kit

Try to refactor the REST API you build in Exercise 1 and reuse your integration tests to verify that the functionality did not change.

### Exercise 4: Manage your entities with a SQL database

### Exercise 5: Consume/Publish events on a message queue

### Questions you might encounter after a while

When to use pointer semantics or value semantics ?  
How to mock dependencies ?  
When to use of interfaces ?  
Error 'failed to cast to AddRequest' does not provide any useful information ?  
What is context used for ?  
How to organize my go program ?  
How to write concurrent go code ?
How to manage channels ?

