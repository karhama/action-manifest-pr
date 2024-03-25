# action-manifest-pr
This action can be used to automatically create manifest PRs into sdk-nrf repo.

## be careful with secrets
This actions is inteded to use NordicBuilder related secret. So triggering
repo will likely have it configured. Secret is used for creating branch and 
manifest PR into sdk-nrf repo. Especially if your repo is having external 
PRs / contributors you should be extra careful triggering this action.
