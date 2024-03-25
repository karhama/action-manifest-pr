# action-manifest-pr
This action can be used to automatically create manifest PRs into sdk-nrf repo.

## be careful with secrets
This action is designed to utilize NordicBuilder-related secret, 
primarily for creating branches and manifest pull requests (PRs) within the sdk-nrf repository. 
Ensure proper configuration of the secret. **Please exercise caution when triggering this action
if your repo has external contributors / PRs.**
