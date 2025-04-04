# Contents

Contains code for part 11 of the [Full stack open](https://fullstackopen.com/en/) course.
This part covers Continous Integration / Continuous Delivery (CI/CD) using Github Actions.
Other parts can be found at and through https://github.com/aaltop/fullstackopen,
with a another CI/CD project at https://github.com/aaltop/fullstack-blogapp-cicd.

A non-exhaustive list of covered concepts:
- CI/CD
    - in integrating code to a version control system, automate
        - linting
        - building
        - testing
        - packaging
        - deployment
- Github Actions
    - workflows that consists of jobs and are triggered by specific events
    - actions
        - perform specific things, like checkout a branch or setup node
        - https://github.com/anothrNick/github-tag-action
        - https://github.com/Jtalk/url-health-check-action
        - https://github.com/rjstone/discord-webhook-notify
    - vars and secrets for Github-side "environment variables"

Fairly simple concepts really. Like writing makefiles, but just a little
more complex. The aim of CI/CD is also fairly obvious: the CI part
ensures that trunk-based development practices are mostly followed,
and the CD part just automates deployment of the code to production.
Overall, the result is speedups in development and lowering of mistakes
due to human error.

## Main technologies introduced

### [Github Actions](https://github.com/features/actions)

Simple enough option for CI/CD. Can be configured to run in Github
repos. Free (with limitations) for public repos.
