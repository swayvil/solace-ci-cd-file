# solace-ci-cd-file
Workflow to push a configuration file to a Solace PubSub+ broker with a validation step
## Prerequisites
### Declare a secret and environment variables
On Github repository settings. How to: [Creating configuration variables for a repository](https://docs.github.com/en/actions/learn-github-actions/variables#creating-configuration-variables-for-a-repository)
#### Declare this secret:
- SEMP_PWD
#### Declare these environment variables:
- MSG_VPN
- SEMP_URL (format should be: https://xxx.messaging.solace.cloud:943)
- SEMP_USER
### Declare an environment
On Github repository settings create an environment named "dev", check "Required reviewers" and add at least one reviewer.
## How to
Under "config" folder, push a configuration file in [Solconfig](https://github.com/flyisland/solconfig) format (json). It will automatically trigger the Github Action workflow. A reviewer will be notified and will have to validate the configuration so it can be pushed on the target Solace service.
![review-deployments](/images/review-deployments.png)
![approve-and-deploy](/images/approve-and-deploy.png)
## References
Another version with a form in input: [solace-ci-cd-form](https://github.com/swayvil/solace-ci-cd-form)
