# SDLC (Software Development Life Cycle)

SDLC refers to different stages software goes through during its development
- Define the problem ("planning")
- Coming up with the map of what the application looks like ("design")
- Psuedocode
- Write the code ("Implementation")
- Test
- refactor (go back and forth between testing/refactor)
- Publish

## Stage Order
Planning -> Analysis -> Design -> Development/Implementation -> Verification/Testing -> Deployment -> Maintenance

## Waterfall
This particular model comes from factory/production line where they produce physical goods and going back/starting over costed a lot of money. The stages (Planning, Design, Implementation, Testing/Verification, Pushing) are done once, and is expected to be as good as they can be. So these are handy for things that have to be super exact (military mission, apollo launches)
But it also came with some drawbacks such as 
    - can't go back and fix so stakes for each stages are high
    - Lack of iteration means that there will be very little change to learn from the testing and reflect the result on the current product
    - Lack of innovation (?)
    - It's inefficient since we aren't always sure what we want exactly.

### Differences between Physical goods and software
Unlike physical goods, it's so much easier to revise/improve software because 1. you can always start fresh (the software doesn't have memory) 2. There is no raw material needed to produce softwares (no limit on raw material)

### Another slight issue with Waterfall is..
The world doesn't stop for you when you are designing/researching/planning and manufacturing your software.

## [Agile](https://agilemanifesto.org/)
Is a set of values to consider when developing software
    
    Individuals and interactions over processes and tools
    Working software over comprehensive documentation
    Customer collaboration over contract negotiation
    Responding to change over following a plan

## Scrum
Is one of the implementation of Agile, and it is characterized by iterations. Unlike waterfall where each stages are gone through once, teams utilizing scrum iterate through those same stages in a rapid manner (every 2-3 weeks). That unit of iteration (2-3 week time span) is called a _sprint_.
In a sprint, we plan the work that seems achievable in upcoming sprint (2-3 weeks worth of work), we design, implement, test, and deploy to production at the end of the sprint.

### Parts of a Sprint
- Sprint planning meeting: you meet together as a team and decide on the scope of the sprint
    - "How much work seems doable in next 2-3 weeks?"
    - "Which feature/bug takes the most priority?"
    - "Any carryover from the last sprint we need to take account of?"

- Daily Standup/Scrum Meeting: During the sprint
    - This is an opportunity to catch up to what everyone else is doing in your team.
    - This isn't a long meeting- supposed to be done in 10 ~ 15 min max standing up the first thing in the morning
    - 3 Questions that gets asked here
        - What did you do yesterday?
        - What do you plan on doing today?
        - Any Blockers? (any issues/items that is blocking You from progressing)

- Burndown Chart
    Using the points assigned to each "user stories"/items we can track how our sprint is going. Comparing the actual remaining points to the projected progress, the team can make adjustments to the sprint.

- Kanban Board
Kanban board is to track each item's movement through different stages.
    - Stages each items go through
        - Product Backlog - Is the big wishlist
        - Sprint Backlog - is the todo list for the sprint
        - Doing - Somebody is actively working on this item
        - Testing - the implementation has been complete, its being tested/code reviewed, some kind of verification process
        - Staging - The verification is done, is ready to be deployed/released
        - Done - The item is officially done
    - Tools we use for Kanban board
        - Trello, Github, Jira, etc.

- Sprint Retrospective
The sprint is now done. The team now meets to discuss how the sprint went
    - How did it go?
    - Any outstanding items?
    - Pacing
    - Challenges
    - What worked well
