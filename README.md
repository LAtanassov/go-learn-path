# Go Learn Path

This repository should guide you the way from the installation of Go till advanced topics like memory management and Go routine scheduler and provide you links to public material.

## Start with the Basics

Lets start with [https://golang.org/](https://golang.org/) and learn the basics.  
A must have here are 
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

### Exercise 1: REST API & Client

Go has a powerful standard library, so let's go and check out the [net/http/](https://golang.org/pkg/net/http/) package.
Build a REST API & Client and write unit/integration/benchmark test cases using [https://golang.org/pkg/testing/](https://golang.org/pkg/testing/).

### Exercise 2: Web App

Go also has a powerful template engine used not only for Web Apps but also in projects like [helm](https://helm.sh/).  
Build a simple Web App with [html/template/](https://golang.org/pkg/html/template/).

## Go kit - A toolkit for microservices

Checkout [Go + Microservices = Go Kit [I] - Peter Bourgon, Go Kit](https://www.youtube.com/watch?v=NX0sHF8ZZgw)
Read more about [go-kit FAQ](https://gokit.io/faq/)

A good starting point are the examples in the repo [https://github.com/go-kit/kit](https://github.com/go-kit/kit)

### Exercise 3: Build REST API using go-kit

Try to refactor the REST API you build in Exercise 1 and reuse your integration tests to verify that the functionality did not change.

### Exercise 4: Manage your entities with a SQL database

### Exercise 5: Consume/Publish events on a message queue

### Questions you might encounter after a while

When to use pointer semantics or value semantics ?  
How to mock dependencies ?  
When use of interfaces ?  
Error 'failed to cast to AddRequest' does not provide me useful information ?  
What is context used for ?  
How to organize my go program ?  
...and many more

