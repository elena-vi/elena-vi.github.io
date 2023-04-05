---
layout: post
title:  "My Micro Frontend Experience"
date:   2023-04-05 14:22:05 +0100
categories: micro frontend
---

As a member of a team that used Micro Frontends, I can attest to their popularity in building web applications due to their flexibility, modularity, and scalability. However, like any new technology, we face challenges when working with Micro Frontends. In this article, I'll share some of the challenges my team and I have faced and how we can overcome them.

One major challenge we experienced was the lack of context. We didn't understand why we were using Micro Frontends because our technical design authority mandated it without explaining the benefits or context behind the decision. This lack of understanding made it difficult for us to be successful, especially when the chosen architecture was used globally and not tailored to a specific problem, causing confusion and implementation challenges.

Another issue we faced was not having enough time to upskill. Our team didn't possess the necessary knowledge and experience with Micro Frontends, which caused delays in development. For example, we didn't understand module federation, a crucial aspect of building Micro Frontends. We also struggled to comprehend how different terraform modules were interconnected and their functions. As a result, our initial deployments didn't work well, leading to wasted time.

Without the proper knowledge of Micro Frontends, we wasted time rebuilding components. We assumed there would be shared components across the ecosystem, but this wasn't always the case. For instance, there was a common app with many components, but we couldn't figure out how to reuse them. Consequently, we ended up rebuilding all those components, wasting time and effort.

Besides the challenges I mentioned, we encountered other difficulties when using Micro Frontends. The infrastructure setup, including terraform setup, DNS, and routing, proved challenging. Pipeline testing wasn't optimised for testing each Micro Frontend independently, resulting in longer deployment times. 

## If I were to face these challenges again, here's how I would overcome them:

Build individual pages as Micro Frontends: Rather than building individual pages in an app, I would make each page its own Micro Frontend. This approach would enable my team to work in parallel and leverage the primary benefits of Micro Frontends. It would also allow for faster data rendering.

Optimise the API: I would optimise the API for Micro Frontends instead of over-fetching data and discarding unnecessary information. This change would lead to more efficient data transfer and faster page loads. Unfortunately, on this particular engagement the technical design authority had forbidden the use of GraphQL.

In conclusion, Micro Frontends can be a powerful tool for building web applications, but they come with their own set of challenges. Teams need to understand the benefits of Micro Frontends, use them effectively, and possess the necessary knowledge and skills to implement them successfully. By overcoming these challenges and adopting best practices, teams can leverage the advantages of Micro Frontends to build scalable, modular, and flexible web applications.
