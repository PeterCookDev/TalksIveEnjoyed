# Talks I've Enjoyed - Agile, Practices, Devops and Testing

## Agile & Development Practices

- [Keavy McMinn - Internal tools: make or break your team](https://vimeo.com/68762928)  [23:00]
Takeaway: Good software is designed around real pain that is pain now. I don't like X - onus on the the individual to put down things they don't like with how to fix it on an ideas portal. 

- [Vasco Duarte - How to improve estimates for software: The #NoEstimates view](https://www.youtube.com/watch?v=7ud-4bKJr8k)  [43:32]

- [Greg Young - How to get productive in a project in 24h](https://www.youtube.com/watch?v=KaLROwp-VDY)  [59:27]
Takeaway: Data mine source control to see how changes to files occur over time. Use NDepend to gather metrics such as afferent and efferent coupling. Metrics are things to look at, not rules which must be upheld.

- [Danielle Sucher - Debugging the Science of Deduction](https://vimeo.com/111108891)  [34:47]
- [Christina Wodtke - The Executioner's Tale](https://vimeo.com/86392023)  [21:36]
- [Kris Gale - Why Yammer believes the traditional engineering organizational structure is dead wrong](https://www.youtube.com/watch?v=RsWZNaaic1k)  [21:32]
- [Dan North - Agile Revisited](https://www.youtube.com/watch?v=pcLbkmvqfiY)  [31:25]
- [Liz Keogh - An Introduction to Cynefin and related awesome thinking tools](https://vimeo.com/144981699)  [44:40]
- [Troy Magennis - Agile Metrics - Beyond Burn Up/Down's onto Metric Driven Coaching](https://vimeo.com/144824390)  [41:17]
- [Ryan McKergow - Retrospectives strike back](https://www.youtube.com/watch?v=MR9kRtQYCu0) [30:04]
- [Doc Norton - Velocity is not the goal](https://vimeo.com/97505655) [1:00:25]

- [Tomek Kaczanowski - Problem-solving techniques for groups](https://vimeo.com/126778448)  [25:29]
Takeaway: Break into smaller groups. Use 5 whys. Use Ishikawa/Fishbone diagrams for breadth first discussions. Use de Bono's thinking hats. Presence of leaders can influence decision making as people don't want to disagree with their leaders. 

- [Aino Vonge Corry - Retrospective Anti-Patterns](https://www.youtube.com/watch?v=Os7_lF6VMXw) [48:52]
Takeaway: To avoid anti-patterns go straight to the problem, deal with problems as they happen not just at retro, focus on issues in the teams control, rotate facilitators, when voting on issues ensure you focus on groups where there are less people as well. 

- [Joakim Sundén - Scaled Agile @ Spotify](https://vimeo.com/111131934)  [43:51

- [Courtney Eckhardt - Complex System Failures and Blameless Retrospectives](https://www.youtube.com/watch?v=Sj0sdbiyatk) [21:43]
Takeaway: Complex systems have complex failures. Human error is not a root cause - how did the system let this thing happen. Remediation items should be a usable change - not try harder or be better! Retrospectives let us understand what the unintended consequences of our decisions were.

- [Patrick Kua - Why Technical Leadership Matters](https://www.youtube.com/watch?v=_6BKK1SPAVI) [42:05]

- [Emily Webber - Communities of Practice, the Missing Piece of Your Agile Organisation](https://www.youtube.com/watch?v=9Owrovki73o) [48:18]
Takeaway: Community of Practice = Group of people who share a concern or passion for something they do and learn how to do it better as they interact regularly. Good insights on how to run a COP and its lifecycle.

- [Paul Rayner - EventStorming - Collaborative Learning for Complex Domains](https://www.youtube.com/watch?v=04tGbixfGEY) [43:36]

- [Ben Rockwood - The Power of A3 Thinking in Action](https://www.youtube.com/watch?v=WoR2CYAwfEM) [26:33]
Takeaway: Kaizen is a way of life not a an event. A3 framework - create a single A3 page. Steps consist of problem statement, problem background (why should anyone care?), current state, desired future state, root cause analysis + gap analysis, define and execute experiments, review and study results against desired future state, decide and act on the new information.

## Testing and TDD

- [Katrina Owen - 467 tests, 0 failures, 0 confidence](https://vimeo.com/68730418)  [27:40]
Takeaway: Outgoing messages assert collaboration occurred. Incoming messages assert the state of the system and side effects. Methods that are hard to test and need characterisation tests are probably doing too much. High code coverage does not mean good tests.

- [Sandro Mancuso - Driving well-crafted code through tests](https://vimeo.com/120567335)  [30:50]

- [Roy Osherove - JS Unit Testing Good Practices and Horrible Mistakes](https://www.youtube.com/watch?v=iP0Vl-vU3XM)  [46:10]
Takeaway: Maybe 1 in 5 tests should have mocks. Should have lots of stubs not mocks. Only mock out dependencies to an external 3rd party framework. Unit tests should avoid logic, random numbers and loops. Watch out for tests that interact.

- [Ian Cooper - TDD, where did it all go wrong](https://vimeo.com/68375232)  [1:00:37]

- [Venkat Subramaniam - Succeeding with TDD: Pragmatic Techniques for effective mocking](https://vimeo.com/68383352) [1:02:09]

- [Todd Gardner - Case Studies in Terrible Testing](https://vimeo.com/144684986)  [35:46]
Takeaway: Code coverage of 0 means you aren't testing, 100% means you really care that you hit 100% but your code could still be bad. Tests might just test how good you are at setting up mocks. Fast to fix is almost as good as never broken. Test what breaks. Test the scariest thing first. Monitoring can sometimes be a substitute for tests.

- [Joe Colantonio - The Test Automation Playbook : Succeeding with Automation Awesomeness](https://vimeo.com/144831370) [32:37]

- [Jimmy Bogard - 8 Simple TDD Rules](https://vimeo.com/111091466)  [41:24]
Takeaway: Add in testing seams, and interfaces when you have multiple implementations only. Don't mock your friends - create testing seams only for the uncontrollable. Use the container for tests - use nested or child containers where you need to swap out instances. Use isolation over faking. Try in memory databases. Test item creation not counts. If your tests aren't helping you ship, stop testing. Allow your approach to change with the context.

- [Seb Rose - So long, and thanks for all the tests](https://vimeo.com/105861375)  [1:00:25]
- [Matt Wynne - Beyond BDD](https://vimeo.com/143941147) [34:32]

## Devops

- [Roy Osherove - Beautiful Builds](https://vimeo.com/97516289)   [56:36]

- [Jez Humble - Continuous Delivery](https://www.youtube.com/watch?v=skLJuksCRTw)  [46:59]
Takeaway: Biggest form of waste is features that are not used (50+%). Aim to optimise for how long to deploy a single line of code to production. Optimise for mean time to restore service rather than no downtime. Test configuration and environmental changes as rigorously as source code. Do side by side release of web services where possible. Database release - batch them up and make sure the running system can work with old and new schemas. Don't build CI in a completely separate CI project.

- [Jez Humble - Stop Hiring Devops Experts and Start Growing them](https://www.youtube.com/watch?v=6m9nCtyn6kE)  [1:37:44]
- [Jez Humble - Adopting Continuous Delivery](https://vimeo.com/68320415)  [47:22]
Takeaway: Hypothesis driven development - smallest amount of work possible to deliver the hypothesis to audience. Keep the system releasable over delivering features. Make the constaint how fast you can analyse the data not how fast you gather it. Continuous Integration is not running jenkins over your feature branches.

- [Jez Humble - (Re-)architecting for Continuous Delivery](https://vimeo.com/68226813)  [1:00:33]
- [Jez Humble - DevOps Culture and Practices To Create Flow](https://www.youtube.com/watch?v=oX8af9kLhlk)  [45:38]

- [Neal Ford - Continuous Delivery for Architects](https://vimeo.com/105751212) [1:01:46]
Takeaway: Fast automated feedback on the production readiness of your app whenever you change infrastructure, code or config. Each stage in the deployment pipeline is an opportunity for feedback. Diamond dependencies - when dependencies of dependencies are different. Prefer choreography to orchestration of services (no 3rd parties such as ESB). Try consumer driven contracts.

- [Rachel Laycock - Continuous Delivery: Tales from the Windowsland](https://www.youtube.com/watch?v=TpzRuUB9r9o)  [48:01]
- [Jennifer Davis - From Hero to Zero](https://vimeo.com/104252736)  [29:05]
- [Damian Brady - .NET Deployment Strategies: the Good, the Bad, and the Ugly ](https://vimeo.com/171950824) [49:01]

## Tools

- [Tim Berglund - Git from the bits up](https://www.youtube.com/watch?v=MYP56QJpDr4)  [55:44]
- [The Motivation for a Monolithic Codebase Why Google Stores Billions of Lines of Code in  a single repository](https://www.youtube.com/watch?v=W71BTkUbdqE)  [30:49]
- [Alex Gaynor - The cobbler's children have no shoes, or building better tools for ourselves](https://www.youtube.com/watch?v=gRFHvavxnos) [29:51]

## Technical Writing
- [Daniel D. Beck - Write the Readable README ](https://www.youtube.com/watch?v=2dAK42B7qtw) [22:49]
- [Tracy Osborn - Writing So Your Words Are Read ](https://www.youtube.com/watch?v=8LiV759Bje0) [29:48]
Takeaway: A lot of documentation is written at the level of the writer not the intended audience. Teach - don't tell. Add really short examples, get them to the success moment as early as possibly.

- [Allison Moore - So You Need to Document an API? ](https://www.youtube.com/watch?v=KSXL-BDoGOw) [30:18]
- [Birgitta Boeckeler - We're Agile, We Don't Do Documentation](https://www.youtube.com/watch?v=UvI3zlv5oUA) [26:03]
Takeaway: Explains some of the reasons that documentation can be valuable, what to keep up to date and why its OK for not all documentation to be up to date. 

- [Martin Gontovnikas - How to Create Good Documentation](https://www.youtube.com/watch?v=lw9R2qMCdqk)  [34:31]
- [Dan Allen - 7 Ways to Hack Your Brain to Write Fluently](https://www.youtube.com/watch?v=r6RXRi5pBXg)  [49:15]
- [A. Jesse Jiryu Davis - Write an Excellent Programming Blog](https://www.youtube.com/watch?v=eHXq-IzlGUE) [26:53]
- [Michael Hartl - Learn Enough Tutorial Writing to Be Dangerous](https://www.youtube.com/watch?v=TpmoxsYeap0) [34:57] 
Takeaway: Process of successive refinement for writing tutorials. Use concrete examples. Asking yourself - What does the reader know at this point in the tutorial?

\* *Disclaimer* - I know this speaker personally.
