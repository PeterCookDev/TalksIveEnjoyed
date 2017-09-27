# Talks I've Enjoyed - Development

## Design Principles and General Development

- [Jimmy Bogard - Crafting Wicked Domain Models](https://vimeo.com/43598193)  [1:03:03]
- [Jimmy Bogard - Solid Architecture in Slices not Layers](https://vimeo.com/131633177)  [55:34]
- [Venkat Subramaniam - The Power and Practicalities of Immutability](https://vimeo.com/131635253)  [1:10:50]
- [Venkat Subramaniam - The Art of Simplicity](https://www.youtube.com/watch?v=-ZPgO5USBoI)  [1:22:32]
- [Sandi Metz - All the Little Things](https://www.youtube.com/watch?v=8bZh5LMaSmE)  [38:46]

- [Michael Feathers - Beyond Error Handling](https://vimeo.com/99668845)  [46:09]
Takeaway: Pervasive error logging gets in the way of reading code. Validate everything upfront and then don't have to do error checking internally. Null checking everywhere is a smell of no trust in private APIs. Avoid exceptions caught way down the call stack where the state is left inconsistent. Want to be able to get back to a state before starting to do the work. If can check in an advance - don't use exceptions. If can't check and you care as its across a system boundary - then use exceptions.

- [Greg Young - The art of destroying software](https://vimeo.com/108441214)  [42:30]
Takeaway: Optimise the building for the deletion of code. Microservices shouldn't need refactoring, they should be disposable. Refactoring should either change tests or the code but not both. Plan to rebuild rather than adapt to change.

- [Greg Young - Unleash your Domain](https://vimeo.com/19428577)  [54:43]
Takeaway: Domain models are not the same as the storage schema. Model state transitions into events. Events are always in the past tense as they have happened. Undo events by compensating events. Command Query separation - A single model cannot be appropriate to reporting, searching and transactional behaviours. Reads happen more than writes, optimise for reads. The domain model is read only.

- [Greg Young - 8 Lines of Code](http://www.infoq.com/presentations/8-lines-code-refactoring)  [45:20]

- [Greg Young - Stop Over-Engineering](https://www.youtube.com/watch?v=GRr4xeMn1uU) [47:25]
Takeaway: Best solution is to not solve a problem. Deliver value not frameworks. Start with the simple happy path and how do I know I am still in it? Then focus on the similarity of the other paths. Iterate. Leave the really complicated bits out as they are probably very rarely used - use manual intervention instead. Don't focus on everything that can go wrong - focus on how you know you are still right. Software is either to save money or make money - know which it is.

- [Katrina Owen - Here Be Dragons](https://www.youtube.com/watch?v=HsWLrSof-ns) [43:42]
- [Katrina Owen - Therapeutic Refactoring](https://www.youtube.com/watch?v=J4dlF0kcThQ)  [26:04]

- [Katrina Owen - Overkill](https://www.youtube.com/watch?v=qLpvc5r6Bb0)  [32:43]
Takeaway: Path to mastery in programming is not well known. Tests are not a proof of your code, they only tell you when you are wrong. Name things by the domain concept - Yell rather than allCaps.

- [Hadi Hariri - Refactoring to Functional](https://vimeo.com/111506976)  [45:00]
- [Mark Seemann - Types + Properties = Software](https://vimeo.com/144800642)  [40:39]

- [Ian Cooper - Not just layers! What can pipelines and events do for you?](https://vimeo.com/113584390)  [1:00:22]
Takeaway: Pipes and Filters used when need to process or transform a stream of data. Each transformation/processing element in the pipeline is a filter. Can be pull based or push based. Can be distributed using messaging channel between filters. Error handling is hard. Different to chain of responsibility as the filters do not execute their successors directly - the pipeline does it.

- [Karoline Klever - What is the actual life expectancy of your code?](https://vimeo.com/142347209) [52:24]
Takeaway: Stop rewriting stuff. Stop adding new frameworks just for the sake of it. Remove dead code and unreachable code. Leave alone legacy code. Legacy = more expensive to maintain than rewriting it

- [James Pearce, Ben Ogle Ben Hamilton - Building an IDE that Scales](https://www.youtube.com/watch?v=WI_Q3PuqAiE) [35:51]
- [Peter Seibel - Engineering Effectiveness at Twitter](https://www.youtube.com/watch?v=8IyXcLFO9ns) [27:52]
Takeaway: Let 1000 flowers bloom then rip up 999 of them. Have a common build system. Aim for 10x offices not 10x engineers. We don't know how to improve engineering effectiveness. Save 5 mins a day for all engineers = 1% gain for the whole organisation. Let people build lots of stuff, see what works, kill the rest.

- [Alan Shreve - Conceptualizing Large Software Systems](https://www.youtube.com/watch?v=2T6Prj82adg)  [17:17]
Takeaway: When exploring a large code base use code coverage tool to work out the minimum set of code that is actually run when you do something. Aim to remove incidental complexity then run on a more complex scenario incrementally to understand more. 

- [Rebecca Sliter - A Tale of Two Feature Flags](https://www.youtube.com/watch?v=rBBLMmr9e-k) [29:34]
Takeaway: Feature flags are not always good - especially when not sure how dependencies scale. Grow exponentially in complexity when you have more than 1 for testing. Feature flags can bleed into unit tests which is bad, removing flags means tests break. Unattended flags are tech debt. Add deadline and maintainer fields to feature flags. When past the deadline automatically branch code, change the config file and cc in the maintainer in the commit/PR.

- [Vaidehi Joshi - A Machine State of Mind](https://www.youtube.com/watch?v=N1jnoPxBGGA) [24:54]

- [John Hyland - Be Awesome By Being Boring](https://www.youtube.com/watch?v=Iheymi5QFEY) [25:34]
Takeaway: Standard is better than better - easy to hire for, stable, easy to google. New tech changes - there may not be tooling, standard usage patterns, more bugs, security wildcard. You need a really good reason to use something shiny. When using shiny - roll out slowly incrementally with a rollback plan in place. Use it for whats meant for. Problems don't add up they multiply - so don't use multiple new techs at once. Non standard technology choices are enormously expensive - you pay for the choice, for the lifetime of the system.

- [Bryan Helmkamp -  Code Quality Lessons Learned](https://www.youtube.com/watch?v=vcH0RBe4Eew) [30:21]
Takeaway: Measuring code complexity with cyclomatic complexity, ABC and LOC. Old code harder to maintan - code matched domain understanding when written, business then diverged. Omega mess - code only has inbound dependencies and doesn't change.

- [Kevlin Henney - Clean Coders Hate What Happens to Your Code When You Use These Enterprise Programming Tricks](https://www.youtube.com/watch?v=FyCYva9DhsI) [1:11:22]
Takeaway: Great example of cargo-culted code being refactored. Smells - noisy logging, mixed levels of abstraction, programming by coincidence and programming by superstition. Comment on a block implies a named block (function).

- [Jim Holmes - "OMG! This Codebase Sucks!" Paying Down Tech Debt While Delivering Value](https://www.youtube.com/watch?v=InCmGFSA3JM) [1:00:21]
Takeaway: 4 part approach to working and evaluating technical debt based around the business value it offers. Evaluate where you are with all stakeholders present. Work out what the business goals are. Measure how bad it is in the code. Improve readability first. Keep using the same metrics when you come to fix things (and after). Everything in dealing with tech debt comes back to organisational culture.

## .NET and `C#`

- [Bart J.F. De Smet - Under the Hood of C# 6](https://vimeo.com/144630847)  [44:25]
- [Kirk Scott Allen - LINQ - Beyond Queries](https://channel9.msdn.com/Blogs/matthijs/LINQ-Beyond-Queries-by-Scott-Allen) [55:03]
- [Kirk Scott Allen - Code Gems From the Rosyln and .NET Source Code](https://vimeo.com/131637370)  [51:51]
- [James Newton-King - Designing Wonderful .NET APIs](https://vimeo.com/97501377)  [1:02:28]
- [Venkat Subramaniam - Transforming your C# code to functional style](https://vimeo.com/97519532)  [1:02:45]
- [Liam Westley - Async C# 5.0 - Patterns For Real World Use](https://vimeo.com/97337304)  [1:07:18]
- [Mads Torgersen - Play in C#](https://www.youtube.com/watch?v=08klj0nZYK8)  [46:53]
- [Cecil Phillip - ASP.NET MVC 6 and the New .NET Web Stack](https://www.youtube.com/watch?v=6wecOOuhSuc)  [55:25]

## Python

- [Andrew Montalenti - NLTK and Text Procesing](https://vimeo.com/53062324)  [40:26]
- [Lynn Cherny - Bestseller Analysis: Sex Scene Detection, Topics, and Pacing](https://vimeo.com/74075845)  [41:36]
- Natural language processing in Python using NLTK [part 1](https://www.youtube.com/watch?v=AOU-Yw1qdJs) [part 2](https://www.youtube.com/watch?v=EuIzZMfHTCg) [part 3](https://www.youtube.com/watch?v=ncUIzVG2zzs)
- [Mariano Anaya - Clean code in Python](https://www.youtube.com/watch?v=7ADbOHW1dTA) [21:44]
- [Brett Slatkin - Refactoring Python: Why and how to restructure your code](https://www.youtube.com/watch?v=D_6ybDcU5gc) [30:24]
- [Stuart Williams - Python by Immersion](https://www.youtube.com/watch?v=RVNIdoepdzU) [3:00:40]
- [Rachel Bunder - I wish I learnt that earlier! ](https://www.youtube.com/watch?v=cy5n6XAtA-w) [29:22]


## Web Development

- [Walter Rumsby - Walter Rumsby on Javascript Testing](https://www.youtube.com/watch?v=TsUdM9UnnL0)  [43:53]
- [Todd H Gardner - Javascript Forensics](https://vimeo.com/133137606)  [50:13]
- [Una Kravets - A Primer on Performance](https://vimeo.com/139912217)  [26:50]

## Microservices, SOA, APIs etc

- [Martin Fowler - Microservices](https://www.youtube.com/watch?v=wgdBVIX9ifA) [26:52]

- [Sam Newman - The Practical Implications Of Microservices](https://vimeo.com/99531595)  [56:10]

- [Sam Newman - Testing and Deploying Microservices](https://vimeo.com/100930174)  [1:03:14]
Takeaway: Independent releasing of microservices - Not a free lunch - complexity increases and testing becomes harder. In tests - use service stubs for downstream dependencies (though it can be painful). Run fake integration tests in production (semantic monitoring). 

- [Damian Brady - The Power of a Great API - The case for writing API first applications](http://tv.ssw.com/6384/the-power-of-a-great-api-the-case-for-writing-api-first-applications-damian-brady-at-ddd-melbourne-2015) [45:02]

- [Fred George - MicroServices: Lessons from 3 Companies](https://vimeo.com/111627195)  [33:05]

- [Darrel Miller - Crafting Evolvable Web API Representations](https://vimeo.com/131643022)  [1:03:19]

- [Mike Amundsen - Learning Client Hypermedia from the Ground Up](https://vimeo.com/131642790)  [54:06]

## Performance and Scalability

- [Sasha Goldshtein - Making .NET Applications Faster](https://vimeo.com/131636651)  [1:01:55]
- [Marco Cecconi - What I've Learnt Working at Scale](https://vimeo.com/144799320)  [40:49]
- [Aaron Stannard - Performance as a First Class Feature with NBench](https://vimeo.com/180862940) [53:51]

## Security

- [Troy Hunt - Hack yourself first: go on the cyber-offence before online attackers do](http://www.youtube.com/watch?v=d_tWyqaQ2Jk)  [52:11]
- [Troy Hunt - 50 Shades of AppSec](https://vimeo.com/153220272)  [1:03:36]
- [Troy Hunt - Lessons from 220 Million Breached Records](https://vimeo.com/154958732) [1:05:11]
- [Troy Hunt - Web Security Essentials by Example](https://vimeo.com/154962595)  [53:09]
- [Troy Hunt & Niall Merrigan - Both Sides of the Attack](https://vimeo.com/154956509)  [1:05:32]
- [Barry Dorrans - Going beyond OWASP](https://vimeo.com/131642364)  [1:01:10]
- [Philip Åkesson, Andreas Hallberg - Secure coding patterns](https://vimeo.com/110897723)  [36:13]
- [Einar Otto Stangvik - Security in the Media](https://vimeo.com/154961992)  [55:12]

## Data Science

- [Ron Bekkerman - Machine Learning: The Basics](https://www.youtube.com/watch?v=wjTJVhmu1JM)  [56:33]
- [Dr. Jim Webber - A Little Graph Theory for the Busy Developer](https://www.youtube.com/watch?v=9Gcjkoaa0ZI)  [51:28]
- [Carina C.Zona - Consequences of and insightful algorithm](https://vimeo.com/137770918)  [39:34]
- [Adam Tornhill - Mine Social Metrics from Source Code Repositories](https://vimeo.com/144670188)  [35:57]

- [Adam Tornhill - Seven Secrets of Maintainable Codebases](https://www.youtube.com/watch?v=0oDporwhToQ) [39:17]
Takeaway: Source control systems hold behavioural data. Need to prioritise tech debt in terms of how often its changed and how often its used. Use LOC (general measure of complexity) and degree of change/change frequency to find hotspots in the codebase. Look for temporal coupling (files committed together regularly) with no obvious explanation - may be copy and pasted code. The number of developers behind a piece of is best indicator of quality problems.

- [Eva Nahari - NLP: Something Old, Something New...](https://www.youtube.com/watch?v=InayOc_Dpyg)  [49:48]

\* *Disclaimer* - I know this speaker personally.
