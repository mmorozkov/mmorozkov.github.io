---
title: "Tailoring Hiring Process"
date: 2022-08-18T16:00:00+02:00
draft: false
toc: false
images:
tags: 
  - hiring
  - interview
---

This write up aims to provide meaningful tips and guidelines for tailoring your hiring routine. It's based on my experience working in mid-size outsourcing company and best advice I could find on the internet.

Most organization have their established ad-hoc processes, thus it's important to understand the basics. Recruitment process seems insidously easy: just hop on a call to talk to a candidate. However, most of the work that increases the quality of the outcomes is done behind the scenes in preparation, precise decision making policy and actionable feedback. And that work start long before the interview.

# Before You Interview Anybody
It's really important to think the whole process through in advance, as it highly impacts how you organize your conversation with a candidate. An interviewer has to understand crystal clear:
- Who they're looking for
- What the new hire would be working on 
- How they're going to make a final decision
- What flow / set of problems would help make that definitive decision
- Whether it's comfortable to communicate and work with the candidate

## Who to Look for
It's much easier when there's one certain job opening in one particular team - then, it must have definitive description of expectations for the successful candidate. But what if you have multiple teams searching for engineers with varying skill sets?

There's a lot of ideas on the internet, and [Joel Spolsky][0] summed it up pretty good: you should be looking for people who
- Are smart
- Get things done

Easy, right? Not so fast, though. This is just the first step to tailor your process to your needs. Smart rarely means 'knows answers to my 100500 random questions about software engineering'.

Also knowing what the new hire would be working on helps tremendously: trim topics and questions down to the most relevant ones. For example, if you're expecting an engineer to write simple CRUD operations over HTTP, you might not need to worry about if they're proficient in transaction isolation levels and/or Java memory model nuances.

## Communication
By far the most overlooked thing in hiring is communication. It might be because, it's hard to objectively measure the comfort level. But it's been stated and proven so many times that one of the major reasons for a project to fail / significantly exceed budget/scope/timelines is bad communication. 

It's absolutely okay to make a `no hire` decision solely based on how bad the conversation was flowing. Like if a candidate is always silent and needs an external nudge in order to talk over a problem, makes horrible judgemental calls (E.g. `only stupid engineers use singletons!`) and expresses a lot of incompatibility with how your teams work is organized, it's totally fine to reject such candidate.

What can help here:
- Let the candidate talk
- Use open-ended questions instead of yes/no ones
- Dedicated short intro call sessions to get to know each other

## Preparation
Ideally, one should have done these by the start of the interview:
- Prepared self-explanatory and self-selling job description
- Read candidate's CV
- Came up with high-level interview plan
- Outlined time constraints for each section
- Prepared most important tasks/questions
- Prepared company/project pitch
- Got familiar with tools and standards for leaving your review
- Watched somebody do it
- Practiced some mock interviews

## After the Interview
The real job starts after you have finished talking with the candidate, no joke! :wink: It's really important to quickly and fully summarize your thoughts on the conversation, make a decision and provide feedback to the candiate

### Candidate Review
One should have same core principles and decision making markers at least within same job description. It's great when you have standardized approach across the company, then you can have a structure and follow same approach for all the interviews.

Best review is done immediately after the interview. In 3 days you vaguely remember the name of the candidate, leave alone what they were good at, what you liked and what they could work on in order to improve. On top of that qualified candidates receive multiple calls a day, so if you're not moving fast, be sure somebody else is!

### Making Final Decision
In the end of the day, as an interviewer you're required to provide a TLDR along the lines of `Grade X, [No] Hire`. Your process, questions you ask, problems you offer to a candidate to solve should pretty much aim at helping you get to a definitive answer to that very question: should I recommend hiring or not. If there's one thing to remember about hiring, it's this: bad hiring is so much worse than not hiring a worthy candidate. Which means it's fine if you reject a good candidate in case you're not convinced, but it's so much more hassle, lost time, money and efforts to fire a mistakenly hired person.

Tips:
- Make the decision binary
    - Avoid `don't know / may be hire`
    - There's just a tiny room for `hire, but to the other team`
- In case of uncertainty lean towards
    - `hire`, when lacking quality candidates and have a lot of positions to fill
    - `no hire`, if the flow of candidates is steady and you are not in a rush to hire just somebody


## Feedback
Any candidate for sure wants to get an offer, but it's not always the case. The next thing on their wish list is feedback. Constructive and actionable one, not a fuzzy BS along the lines of `we don't feel confident you'll be able to follow through on projects of our usual magnitude`.

But why would you as an interviewer care? First off, it's to show extreme professionalism and engage candidates further. Since when one feels treated poorly they make it heard out loud: whining to the friends, leaving negative reviews about their experience, etc. As a result, such candidates never come back, don't recommend friends and discourage everybody else to engage in talks with you. And it all can rather simply be avoided by following good will principles:
- Level the expectations: let a candidate know during the interview when they can expect the feedback. The sooner, the better.
- Let them know on the spot how the interview went, at least in general
- Make feedback actionable, compare these:
    - no understanding of technology XYZ whatsoever → take on this short online crash course that explains how XYZ works
    - doesn't understand nuances of ABC → read this book and those blog posts to get better understanding and dive deeper in ABC, continue with coding exercises on that platform
    - doesn't write / writes poor tests → watch this presentation on testing pyramid, read this write up on what constitutes a great unit test, make yourself familiar with BDD through cucumber learning center

It will do wonders: candidates will remember you, will be glad to talk to you again, an will likely recommend to others. And it literally takes less than 5 minutes of your time.

# Now What
Recruitment process seems insidously easy: just hop on a call to talk to a candidate. However, most of the work that increases the quality of the outcomes is done behind the scenes in preparation, precise decision making policy and actionable feedback.

Next we'll catalogue all the different ways and stages of a technical interview.

[0]: https://www.joelonsoftware.com/2006/10/25/the-guerrilla-guide-to-interviewing-version-30/