# solace-ci-cd-file
Workflow to push a configuration file to a Solace PubSub+ broker with a validation step
## Prerequisites
### Declare a secret and environment variables
How to: [Creating configuration variables for a repository](https://docs.github.com/en/actions/learn-github-actions/variables#creating-configuration-variables-for-a-repository)
#### Declare this secret:
- SEMP_PWD
#### Declare these environment variables:
- MSG_VPN
- SEMP_URL (format should be: https://xxx.messaging.solace.cloud:943)
- SEMP_USER
## References
Another version with a form in input: [solace-ci-cd-form](https://github.com/swayvil/solace-ci-cd-form)
