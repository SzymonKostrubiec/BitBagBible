### Events:
1. Builds must work for bellow events:
    - push
    - pull request
    - release, where releases has type 'created'.

   #### Example code:
   ```YML
      on:
        push:
          branches-ignore:
            - 'dependabot/**'
        pull_request: ~
        release:
          types: [created]
        schedule:
          -
            cron: "0 1 * * 6"
        workflow_dispatch: ~
   ```
### [Previous chapter]('./doc/GithubBuilds/2_EventsSubchapter.md') / [Main page]('./doc/GithubBuilds/GithubBuilds.md') / [Next chapter]('./doc/GithubBuilds/3_JobsAndStrategySubchapter.md')