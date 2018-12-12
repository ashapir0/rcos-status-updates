## Looking back on a successful semester

This semester in RCOS presented several interesting challenges both managerially and technically.  Developing V2 of Parking Ticket Appeals Management encompassed a ground-up rebuild.  Working with Dylan, Josh and Will on architecture at the start of the semester was a pleasure and in my opinion we came up with a robust, sustainable and elegant solution.

Starting with our database, Josh and I worked together to tweak and remove redundancies in our data-models.  We created UML diagrams, and worked with Dylan to implement migrations with [node-pg-migrate](https://github.com/salsita/node-pg-migrate).  Figuring out how to structure large migrations was challenging and I think we can still improve in this area.  However, from V1 to V2, developer onboarding, CI/CD and deployment were immensely streamlined with migrations.

The use of TypeScript across the ecosystem (my decision) has aided greatly in the cohesion of our codebase and the code-contracts across services.  While there is more overhead upfront working with TypeScript, again I think there was a massive payoff.

In terms of our backend structure, I again think we made great strides.  Our codebase makes much better use of abstraction and is very loosely coupled and highly cohesive.  This leads me into a good portion of my time, my [logical-cas-client](https://github.com/ashapir0/logical-cas-client).  I found that in the previous version of the project, authentication was a massive issue and was woefully insecure.  I hope to continue working on the [logical-cas-client](https://github.com/ashapir0/logical-cas-client) in the future to support other versions and SAML.

We also now have high coverage unit and integration tests written by myself, Josh, Will and Dylan.  These will lay the way for this project to become very stable in the future.

On our frontend React with TypeScript and MobX was a perfect mix.  Although refactoring needs to be done and automated tests need to be put in place, there is now a solid foundation.

### My Contributions
[40+ Service Commits](https://github.com/rpi-ptam/ptam-service/commits/master?author=ashapir0)

[15+ Client Commits](https://github.com/rpi-ptam/ptam-client/commits/master?author=ashapir0)

[8 Migrations Commits](https://github.com/rpi-ptam/schematron/commits/master?author=ashapir0)
