# Good tool
Add this to `.github/workflows/sync.yml`. It will keep your forks in sync with the original one.

```
name: Sync Fork

on:
  schedule:
    - cron: '00 00 * * *' # sync the repo everyday at 00:00 UTC!
  workflow_dispatch: # on button click

jobs:
  sync:

    runs-on: ubuntu-latest

    steps:
      - uses: tgymnich/fork-sync@v1.4
        with:
          owner: SwannedLakee
          base: master # this should match  actual name of the branch (check it with the original repo)
          head: master # this should match  actual name of the branch (check it with the original repo)
```
- 👋 Hi, I’m @SwannedLakee
- 👀 I’m interested in Drama and Film Production
- I just started learning coding

