---
layout: post
title:  "Micro Frontends: Challenges Faced by Teams"
date:   2023-04-05 13:22:05 +0100
categories: jekyll update
---
Micro Frontends have become a popular approach in building web applications due to their flexibility, modularity, and scalability. However, like any new technology, there are challenges that come with it. In this article, the challenges faced by teams when using Micro Frontends and possible solutions to overcome them will be discussed.

## Background

Two main approaches to building websites have emerged in recent years Single Page Apps and micro frontends, each have advantages and disadvantages, in short single page apps create a community of engineers working in a single application this means it’s very easy to share solutions such as components, libraries and optimisations but merge conflicts can be a problem as larger teams try to contribute to the same app. Micro frontends, like microservices are multiple apps making it easy for several teams to build their own apps without getting in each other's way but it’s then harder to share components, libraries and optimisations.

## Lack of Context

A major challenge faced by teams when using micro frontends for the first time without proper context is the lack of understanding of why they are being used. For example, if a technical design authority mandates the use of micro frontends without explaining the benefits or context behind the decision, it can make it difficult for the team to be successful. Moreover, if a chosen architecture is used globally and not specific to a particular problem, it can lead to confusion and challenges in implementation.

## No Time to Upskill

Another challenge is the lack of time to upskill. Teams may not have the necessary knowledge and experience with Micro Frontends, and this can cause delays in development. For instance, they may not understand module federation, which is crucial for building Micro Frontends. Also, the team may not know how the different terraform modules are interconnected and what they do. As a result, the first few deployments may not work well, leading to wasted time.

## Wasted Time Rebuilding Components

Without the proper knowledge of Micro Frontends, teams may waste time rebuilding components. They may assume that there will be some shared components across the ecosystem, but this may not be the case. For example, there may be a common app that includes many components, but it may not be clear how they can be reused. Therefore, the team may end up rebuilding all those components, leading to wasted time and effort.

## Other Challenges

Aside from the challenges mentioned above, other difficulties may arise when using Micro Frontends. These include:
- Infrastructure setup, such as terraform setup, DNS, and routing, can be challenging.
- Pipeline testing may not be optimised for testing each Micro Frontend independently, leading to longer deployment times.


## Some ways they could overcome the challenges

If a team were to face the same challenges, here are some ways they could overcome them:

### Foster Clear Communication and Documentation Practices

Clear communication and documentation are crucial for successful Micro Frontends implementation. Through workshops, documenting project rationale, and creating best practice guidelines, teams gain comprehensive knowledge, enabling informed decisions and effective architecture implementation.

### Building Individual Pages

Instead of building individual pages in an app, each page would have its own Micro Frontend. This would allow the team to split the work up amongst themselves and work in parallel, which is one of the primary values of Micro Frontends. It would also be faster to render the data.

### Building a deployment platform

Instead of leaving teams to attempt to reuse existing solutions to move to a Micro Frontend approach, build a standard infrastructure configuration and deployment pipeline optimised for building, testing and deploying a set of Micro Frontends. This allows for testing to be optimised and tests to be run in parallel, this could support either a monorepo or polyrepo solution allowing shared code to be accessed by each Microfrontend more easily.

### Optimising the API

The API providing data could be optimised for the Micro Frontends by using GraphQL, rather than pages over-fetching and getting everything from the API and throwing away the data that wasn't needed. This would lead to more efficient data transfer and faster page loads. 

## Conclusion

Micro frontends can be a powerful tool for building web applications, but they come with their own set of challenges. Teams must understand the benefits of micro frontends, how to use them effectively, and have the necessary knowledge and skills to implement them successfully. By overcoming the challenges and adopting best practices, teams can leverage the benefits of micro frontends and build scalable, modular, and flexible web applications.

