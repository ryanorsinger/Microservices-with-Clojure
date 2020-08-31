# What
- Multiple, small web services vs. a single monolithic application

## Why
- Lower total cost of ownership/maintenance (in specific situations)

## Examples of Monolithic Architecture
- An example of a monolithis application is Microsoft Word which is installed through a single deployable artifact. All of the copmonents work together.
- Separation of Concerns
- "Distributed Monolith"
- The standard 3 tiered application - Presentation, Business Logic, Persistence 
- Even though a monolitic application is built on separation of concerns, it's still a single application on a single stack that provides all the services to its users.
- Not possible to scale each service independently

## Introducing Microservices
- Each service does _only_ one job and does it well. 
- Each service has its own database, its own schema, and provides access to data and services through APIs.
- Instead of layers, each service is organized around a bounded context
- Similar to a Service Oriented Architecture but uses HTTP instead of any message oriented middleware
- "Architectural Style of Microservices is referred to as fine-grained SOA, perhapse service orientation done right" - Martin Fowler

## Terminology

## When
- When the productivity of the team starts decreasing when changes to the monolithic application start affecting more than one component, you might want to consider Microservices.

## Guidance
- If you can, refactor before dis-integrating your application into microservices.
- Again, microservices should come after refactoring

## Examples of Migrations to Microservices
- Amazon's original Perl monolith
- Twitter's Ruby on Rails monolith

- Continuous integration
- Continuous delivery pipelines
- Automated deployment, scaling, and monitoring of services for real-time feedback

## How
- Organize microservices around business capabilities or database access patterns. 
- Also look for areas like authentication, authorization, and notification that can be perffected oas a service and can be leveraged by one or more microservice later.