# Talks I've Enjoyed - Agile, Practices, Devops and Testing

## Agile & Development Practices

- [Keavy McMinn - Internal tools: make or break your team](https://vimeo.com/68762928)  [23:00]
Takeaway: Good software is designed around real pain that is pain now. I don't like X - onus on the the individual to put down things they don't like with how to fix it on an ideas portal. 

- [Vasco Duarte - How to improve estimates for software: The #NoEstimates view](https://www.youtube.com/watch?v=7ud-4bKJr8k)  [43:32]

- [Greg Young - How to get productive in a project in 24h](https://www.youtube.com/watch?v=KaLROwp-VDY)  [59:27]
Takeaway: Data mine source control to see how changes to files occur over time. Use NDepend to gather metrics such as afferent and efferent coupling. Metrics are things to look at, not rules which must be upheld.

- [Christina Wodtke - The Executioner's Tale](https://vimeo.com/86392023)  [21:36]
Takeaway: Ideas are cheap, execution is everything. OKRs - Objectives and Key Results. Objective = dream (qualitative), Key Result = success criteria (quantitative). Need to have regular checkins with the team. Have 3 priorities for the week. What is the confidence in the quarterly OKRS. What are the projects in the next 4 weeks. What are your measures of organisational health? Are you pushing people too hard? Celebrate every Friday - everyone needs bragging time.

- [Kris Gale - Why Yammer believes the traditional engineering organizational structure is dead wrong](https://www.youtube.com/watch?v=RsWZNaaic1k)  [21:32]

- [Dan North - Agile Revisited](https://www.youtube.com/watch?v=pcLbkmvqfiY)  [31:25]

- [Liz Keogh - An Introduction to Cynefin and related awesome thinking tools](https://vimeo.com/144981699)  [44:40]

- [Troy Magennis - Agile Metrics - Beyond Burn Up/Down's onto Metric Driven Coaching](https://vimeo.com/144824390)  [41:17]
Takeaway: Use combinations of competing metrics to stop people gaming the system. Quadrant approach - do it fast, do it on time, do it right, keep doing it. People won't try to change a number they don't understand. Measure the team not individuals. Aim for leading indicators that are passively captured. When comparing with other teams - show no numbers, show trend only against trend for company. Give coaching strategies based on the trendline they have.

- [Ryan McKergow - Retrospectives strike back](https://www.youtube.com/watch?v=MR9kRtQYCu0) [30:04]

- [Doc Norton - Velocity is not the goal](https://vimeo.com/97505655) [1:00:25]
Takeaway: Goodharts Law - "When a measure becomes a target, it ceases to be a good measure." can lead to paying people for the wrong behaviour. How you get there is more important than getting there. The Hawthorn Effect - when you say are you watching something it will improve. Velocity vs code complexity - as code becomes more complex the slower the team becomes. Measure many things - scorecards, velocity, code quality, avg hours applied to the project, team joy in the pre commit hook - 0 (I hate this code) - 5 (this code is so awesome it should be open sourced). Metrics are not for managers, they are for the team.

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
Takeaway: A test case per class fails to capture the ethos of tdd. The trigger for a new class is implementing a new requirement. Only test the surface of a module. Unit tests run in isolation from other tests, not other modules. Databases, file systems stop tests being isolated from each other. Tests should not depend on implementation details. Don't mock out your internals. Mock the port to the adapter not the adapter itself.

- [Venkat Subramaniam - Succeeding with TDD: Pragmatic Techniques for effective mocking](https://vimeo.com/68383352) [1:02:09]

- [Todd Gardner - Case Studies in Terrible Testing](https://vimeo.com/144684986)  [35:46]
Takeaway: Code coverage of 0 means you aren't testing, 100% means you really care that you hit 100% but your code could still be bad. Tests might just test how good you are at setting up mocks. Fast to fix is almost as good as never broken. Test what breaks. Test the scariest thing first. Monitoring can sometimes be a substitute for tests.

- [Joe Colantonio - The Test Automation Playbook : Succeeding with Automation Awesomeness](https://vimeo.com/144831370) [32:37]

- [Jimmy Bogard - 8 Simple TDD Rules](https://vimeo.com/111091466)  [41:24]
Takeaway: Add in testing seams, and interfaces when you have multiple implementations only. Don't mock your friends - create testing seams only for the uncontrollable. Use the container for tests - use nested or child containers where you need to swap out instances. Use isolation over faking. Try in memory databases. Test item creation not counts. If your tests aren't helping you ship, stop testing. Allow your approach to change with the context.

- [Seb Rose - So long, and thanks for all the tests](https://vimeo.com/105861375)  [1:00:25]
- [Matt Wynne - Beyond BDD](https://vimeo.com/143941147) [34:32]
- [Caitie McCaffrey - The Verification of a Distributed System](https://www.youtube.com/watch?v=ZDQdF6WCt2w) [41:22]
Takeaway: Array of techniques to test in the wild such as integration, unit, property based testing, fault injection etc. Unit tests need to cover error handling - 35% of catastrophic failures happen due to bad error handling. Passing tests doesnt mean your system is correct.

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

- [Damian Brady - .NET Deployment Strategies: the Good, the Bad, and the Ugly ](https://vimeo.com/171950824) [49:01]

## Tools

- [Tim Berglund - Git from the bits up](https://www.youtube.com/watch?v=MYP56QJpDr4)  [55:44]

- [The Motivation for a Monolithic Codebase Why Google Stores Billions of Lines of Code in  a single repository](https://www.youtube.com/watch?v=W71BTkUbdqE)  [30:49]

- [Alex Gaynor - The cobbler's children have no shoes, or building better tools for ourselves](https://www.youtube.com/watch?v=gRFHvavxnos) [29:51]
Takeaway: We build big frameworks, but we don't build little tools for ourselves. Implement processes by a computer rather than by hand as it means no ambiguity in what the process is or does as its code. Examples of using github3 api in python.

## Technical Writing

- [Daniel D. Beck - Write the Readable README ](https://www.youtube.com/watch?v=2dAK42B7qtw) [22:49]

- [Tracy Osborn - Writing So Your Words Are Read ](https://www.youtube.com/watch?v=8LiV759Bje0) [29:48]
Takeaway: A lot of documentation is written at the level of the writer not the intended audience. Teach - don't tell. Add really short examples, get them to the success moment as early as possibly.

- [Allison Moore - So You Need to Document an API? ](https://www.youtube.com/watch?v=KSXL-BDoGOw) [30:18]

- [Birgitta Boeckeler - We're Agile, We Don't Do Documentation](https://www.youtube.com/watch?v=UvI3zlv5oUA) [26:03]
Takeaway: Explains some of the reasons that documentation can be valuable, what to keep up to date and why its OK for not all documentation to be up to date. 

- [Martin Gontovnikas - How to Create Good Documentation](https://www.youtube.com/watch?v=lw9R2qMCdqk)  [34:31]
Takeaway: Writing documentation for developers - specifically API documentation. Developers don't like prose - we like code snippets you can copy and paste. Use the documentation site to automatically configure the downloads of code to include any configuration for the user. People get your documentation from everywhere - use markdown on Github and markdocs. Have a complete GitHub readme. Things should be easy to find - couple of clicks to find information. Use numbered steps, be concise include a lot of code.

- [Dan Allen - 7 Ways to Hack Your Brain to Write Fluently](https://www.youtube.com/watch?v=r6RXRi5pBXg)  [49:15]
Takeaway: Write in plain text to tranlsate thoughts in purest form. Use questions to drive out sentences. Use a sentence per line - loses line breaks in markdown and is easier to diff. Draft in comments - todos, comments as you write etc. Visualise progress using the preview. Use source control to review changes. Read on a small screen away from your desk.

- [A. Jesse Jiryu Davis - Write an Excellent Programming Blog](https://www.youtube.com/watch?v=eHXq-IzlGUE) [26:53]
Takeaway: Writing is super powered thinking. Write essays rather than blog posts - they last longer and not obliged to write constantly. Write short things - 3 paragraph book review. 

- [Michael Hartl - Learn Enough Tutorial Writing to Be Dangerous](https://www.youtube.com/watch?v=TpmoxsYeap0) [34:57] 
Takeaway: Process of successive refinement for writing tutorials. Use concrete examples. Asking yourself - What does the reader know at this point in the tutorial?

## Debugging

- [Danielle Sucher - Debugging the Science of Deduction](https://vimeo.com/111108891)  [34:47]
Takeaway: Make it fail. Simplify by ruling out whats not involved.  Form a hypothesis. Separate facts from interpretation - keep a list of facts. Divide and conquer. One change at a time. Keep an audit trail of what you've tried and what it did. If you didn't fix it, it ain't fixed. How to use git bisect for working out when a bug was introduced.

- [Alex Gaynor - Techniques for Debugging Hard Problems](https://www.youtube.com/watch?v=ij99SGGEX34) [28:08]
Takeaway: Hard problems - timing or ordering dependent, cross module/library boundaries. Everything is in scope to be the cause (though unlikely to be the compiler). Read all the source. Trust nothing - verify everything. Use OS tracing, logging, debugger, IDE (its all about reading code), Grep, domain specific tools, instrumentation. Pair debug. Complex systems rarely break with a single cause.

\* *Disclaimer* - I know this speaker personally.
