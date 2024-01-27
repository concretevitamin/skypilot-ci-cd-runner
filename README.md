# SkyPilot in GitHub Action

*Testing: Adding some random commit to test the CI/CD in PR*

GPU CI/CD runner that works.

- Run tests on any GPU VMs on the cloud in GitHub Action
  - Launched in your cloud accounts
  - Use any GPUs
  - Lowest cost
- Auto-cleanup
  - Test VMs automatically shut down themselves
  - Test cancellations do not leave VMs running

## Setup (GCP)

- Create service account with appropriate permissions
- Test run `sky launch` using that service account on your laptop
- Add two env vars to repo secrets
  - `GCP_PROJECT_ID`
  - `GCP_SERVICE_ACCOUNT_KEY`
![](https://i.imgur.com/pjBgPGk.png)

## Successful run example

![](https://i.imgur.com/HjNGtuG.png)

## Cancellation example

![](https://i.imgur.com/KaVFYtT.png)
