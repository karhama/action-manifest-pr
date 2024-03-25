# action-manifest-pr
This action can be used to automatically create manifest PRs into sdk-nrf repo.

## usage
You can call this workflow in your repository to automatically create manifest PRs.

```yaml
name: Create manifest PR
on:
  pull_request:
    types: [opened, synchronize, closed]
    branches:
      - main

jobs:
  call_workflow:
    uses: nordicbuilder/action-manifest-pr/.github/workflows/auto-manifest-pr.yml@main
    secrets:
       NB_TOKEN: ${{ secrets.NORDICBUILDER_TOKEN }}
```

## about secret
This action is designed to utilize NordicBuilder-related secret, 
primarily for creating branches and manifest PRs within the sdk-nrf repository. 
Ensure proper configuration of the secret in calling repository.
**Please be careful when using this action in public repos i.e. make sure it's not triggered for outside contributors**

