# Le Wagon Prep: Startup Technical Workflow

## What is a Startup?

- See Lean Startup by Eris Reis
- A startup is a temporary organizatiion formed to search for a repeatable and scalable business model
- When you found a business model, you cease to be a startup

## Versioning

- Backup versions of your work and track modifications.
- A way to roll back changes, share and collaborate
- Code Versioning tools Github, Gitlab, Gitbucket
- Cloud storage has versioning: Google Drive/ Docs, Box.com, Dropbox

## Collaborating

- Work as a team on the same project on different **branches**
- One branch = one feature
- pull request - you're asking your team to review your work and merge it to the Github master branch
- Submit your work on GitHub through **pull requests**
- **Review** the code & **merge** the branches

## Continuous Deployment

- Deployment is pushing the latest version of Github master branch to a production server
- Deploy your app in production with quick command lines
- Continuous delivery ensures minimal impact from bugs, and fast feedback from users
  - you write tests, write code and as soon as your code is ready (tests passed), it gets pushed to production
  - If you push code regularly (hourly/ daily), you only risk breaking small parts of your application
  - If you push code every 3 months i.e. lots of changes/ new features in one release, the chance is high that you'll break a lot of stuff

## Testing and Monitoring

- Never push your code without testing!
- Old school Dev Teams have a separate QA team, but this doesn't make sence - as a developer, if you're not testing your code, you're not doing your job
- You should write tests for every feature
- TDD = write unit tests, then write code that fulfills the requirement and passes the tests
  - TDD is more important for projects that don't have visual feedback e.g. a creating Ruby library (no visual feedback) versus a website (visual feedback from browser) -
- Implement Test-Driven Development (TDD) to avoid huge future technical debt
- Shipping features without test builds up technical debt that builds up into something unsustainable such that eventually the entire codebase would need to be refactored
- Implement bug tracking and reporting
- [Travis CI](https://travis-ci.org/) automatically tests every commit pushed on every branch in Github, marks commits as green (pass) or red (fail) and sends email notifications
- [UptimeRobot](https://uptimerobot.com/) monitors your websites uptime

## Back Up Your Data

Prevent the loss of data with automatic backups of your database.

## Resources & Tools

[Slack](https://slack.com/intl/en-ae/) for internal communications
[Trello](https://trello.com/en) for product management
Versioning and collaboration on [Github](https://github.com/)
Deployment on [Heroku](https://www.heroku.com/)
[Travis CI](https://travis-ci.org/), your production tests runner
Bug tracking: [AppSignal](https://www.appsignal.com/) & [Raygun](https://raygun.com/)

## Advice from a Developer

- resist meta-work
  - work/ meetings to talk about work
- avoid meetings
  - even Scrum standups
- write everything down
  - i.e. more people will see it in Slack that hear you say it, and everyone will be on the same page
- Embrace Asynchronicity
  - if you write everything down you can be asynchronous
  - you get stuff to do and you do it at the right time
  - work does not get done at the same place and the same time
  - important for a globally distributed workforce
- Don't pull me from _The Zone_ / state of _Flow_
