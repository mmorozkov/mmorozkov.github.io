---
title: "Power of Tiny Continous Improvements"
date: 2023-04-04T16:00:00+02:00
draft: false
toc: false
images:
tags: 
  - leadership
  - management
  - continous improvements
---

Most IT managers and leaders have seen their share of engineering teams that struggle with different large scale problems, like poor code quality, no test coverage, slow code reviews and many others. Often times, teams either back off and settle with what they have or try to fix everything everywhere all at once. Neither seems to be a silver bullet and a great response, as I think there always should be some middle ground. In this write up I want to share an experience of one of the engineering teams I worked with, how tiny continuous improvements could yield great results over time.

# Where We Were
A while back, one of my development teams inherited a proof-of-concept type of project, that our organization wanted to launch in production soon. The team had practically zero prior knowledge of the product, but still had to take over the existing code base and seamlessly continue working towards the roadmap without losing a single bit. One of the first chalelnging tasks was to understand what we had at hand with little documentation and understanding of architecture decisions made in the past.

As time passed by, our velocity didn't seem to increase much though. Thus, we decided to discuss and address that particular issue  at one of our technical retrospectives. The team was too quick to converge on the issue of slow code reviews: it was about 10 calendar days on average between PR creation and merge. The team suggested several potential improvements, such as tagging the necessary people in Slack, starting and ending the workday by reviewing open pull requests, creating necessary automation for alerting, and so on. 

# Finding the Root Cause
While the team and I gradually tried to implement new practices, we were constantly monitoring their impact through our metrics. The time for the first review steadily was reducing. However, surprizingly the team members privately were still rasing issues about the review speed, which made my concerns growing that we were not treating the illness rather just addressing the symptoms. After a series of team tech minutes and 1-1 meetings I had with each team member, I was finally able to formulate a new hypothesis: it wasn't about the code review speed per se, but rather a general team's feeling of a huge insecurity about the overall confidence over their work.

When this idea was expressed publicly in front of the team, it actually turned out to be so true, as if folks were only waiting for someone to bring that uncomfortable though to the light! They addmited they were absolutely unsure about the quality of their code, and code reviews were serving as a safety net for the engineers to simply share the responsibility for delivering features with someone else from the team! It was a crucial point for all of us to have an AA-style sitdown to admit we had a bigger problem than just a review speed.

# Plan
Now that we got the problem statement and analysis, the team was able to brainstorm the ideas and approaches that could help and finally we came up with the specific steps and action plans. Ultimately, We decided that in order to conquer the initial problem of insecure ownership of the code, we needed to attack it from 2 angles. 

Firstly, we needed to build an automation safety net, so that we can detect potential defects as soon as possible. Which would allow us to have enough time to addresss them and to increase the confidence of stability of the new changes. And on the opposite site, green automation would raise internal confidence over quality.

Secondly, we wanted to shift from `just maintaining` mentality to `fully owning` one, where there's no room for lousy excuses like "it's been that way for a very long time and it was fine, let's leave it as-is". Whereas on the contrary, the team is rather focused on constantly improving the product.

# Building Automation
Digging deeper here, we outlined 4 main points of attack:

1. **Automated Tests**

At some point we admitted that the team hardly wrote any automated tests. Why? There was already a lot of code written, and the product manager kept adding more features, with a great desire to reduce time-to-market. Each team member acknowledged that they wanted to write tests, but it was challenging to start with the very first one. Also, there was a common concern about time and estimates, as team believed that writing tests takes a long time, while the product manager demands more features and faster!

Firstly, I conducted several sessions with the team regarding tests and TDD approach in particular. We read and thoroughly discussed Kent Beck's [TDD by Example][2]. Additionally, through networking, we managed to pay an open doors visit to a fellow company, where all the teams work in pairs using TDD for 40 hours a week. It was a great experience for the team to actually meet and talk to real people who employ these techniques. 

2. **Practicing XP Techniques**  

We also got a great advice there — to read arguably the best book for engineers, that is [Agile Technical Practices Distilled][0], and complete all the Kata exercises the authors suggested after each chapter. Within next few weeks, the guys completed almost all the exercises from the book in pair programming and TDD mode. Here, the team started to doubt the initial statement of "writing tests takes a very long time" Yes, it takes some extra time, but you win it back with interest because you need to debug corner cases or solve defects that your original code generated less frequently.

Then, at one of the retrospectives, the team agreed to try pair programming for the product development. Over the next four months, the guys worked using the Pomodoro method for 6 hours a day, with each hour consisting of three 20-minute splits, constantly switching navigator-driver roles in pairs. After just two weeks of the experiment, the team realized that code reviews were faster, if not fully obselete and redundant, because they caught errors earlier in the development process, and their code was intrinsically being reviewed as it was written.

3. **Employing CI/CD Tools**

The next step on the menu was to create proper CI/CD pipelines to ensure compatibility and correctness of the new changes, along with being able to deploy several times a day and quickly recover in case of errors.

As we progressed with this endeavor, the team realized some impediments within the system and design department, that we no longer needed to uphold. The main one being the monolithic architecture — when one of the smaller services was receving an update the whole product had to be subjected to CI pipelines and redeploy. As a result within next few months we were able to extract vital microservices and ensure CI + CD of a particular service to be under 10 minutes.

Moreover, we also started measuring our test coverage through SonarQube and introduced automated linters to fail our PRs, if there's an obvious code smell there.

4. **SRE Practices to Instill Ownership**

Last but not least, we decided to put emphasis on actually owning the product. Here we havily relied on SRE principles that Google greatly described in their [SRE books][3]. We started with defining some service level objectives we wanted to achieve. That in turn, demanded for more granular logging, monitoring and prompt timely alerting.

At first we were overwhelmed with the number of errors and messages we were receiving. However, it also gave us in impulse to fine-tune our alerting to reduce the number of false positives. We also decided to adjust our logging levels, so that errors would represent only things that require immediate attention. And consequently, that allowed us to narrow down some specific defects and fix them to again increase the overall confidence level.

Later on we introduced support duty days, when software engineers would plow through incidents, support tickets and production errors as their first priority task on some rotation schedule. Not only did it allow us to decrease the volume of potential problems and improve our automation, but also we were able to increase the bus factor for a lot of services of our product, as being on duty prompted folks to dive deeper in all the areas of the application

# Results
There's absolutely no doubt that neither of the ideas and changes above would make a huge difference for the overall speed, quality and confidence of the team. However, the volume of those changes and established and adopted process of generating and reviewing new ideas, implementing action items and measuring the impact accumulated for much greater results.

We started with a monolith, 10 business days for a PR review on average, long cycle time (due to lots of big tickets ~week+ of work) and 0 tests, little automation and monitoring. In 3 years we had 15 separate services, 70% test coverage, cycle time below 2 days, 50+ CI/CD pipelines automating testing and deployments, with 3-5 deploys to production per day.

It was about identify the root of the problem, getting the team on board with an idea to incrementally become better, establishing processes for continous improvement, and providing the team and the engineers with means, tools and authority to make those changes happen!

[0]: https://www.packtpub.com/product/agile-technical-practices-distilled/9781838980849
[1]: https://martinfowler.com/articles/ship-show-ask.html
[2]: https://www.amazon.com/Test-Driven-Development-Kent-Beck-ebook/dp/B095SQ9WP4
[3]: https://sre.google/books/