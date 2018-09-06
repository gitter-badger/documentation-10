## Development Process

We follow the `gitflow` process, more detailed information can be found [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

Each new feature (or hotfix etc) should be opened in a new branch with the type of branch, followed by a `/` and then the name of what is being worked on. I.e.

    feature/login-page

or

    hotfix/loading-timeout

When work is finished, a `PR` **must** be created and the work will then be reviewed by another member of the team. 
In order to be merged, a PR must:

1. Have tests written for the work done (unit and e2e)
2. Report a passing build by Travis
3. Have documentation for any new files or features
4. Pass the code review

## Code Review

A code review can involve feedback in person or be provided in the comments to the `PR`. A branch can not be merged until this has passed.`

