# ecsconnector
Script used for connecting to AWS ECS tasks:

```
~/c/ecsconnector (main)> ecsconnect
Which profile would you like to use? (default: cdk-production)
1) default
2) west
3) internal-products-subaccount
4) cdk-staging
5) cdk-production
Choice (just hit enter for default): 5
You have selected profile cdk-production

Using selected profile cdk-production
Using region us-east-1

Which cluster would you like to connect to?
1) default			  6) qa-pubapp
2) demo-pubapp			  7) soundon-pubapp
3) production-data-platform	  8) staging-data-platform
4) production-pubapp		  9) staging-pubapp
5) production-royaltyestimator	 10) staging-royaltyestimator
#? 4
You have selected cluster production-pubapp
The production-pubapp has the following services available:
1) caddy-production-pubapp	3) fluentbit-production-pubapp
2) django-production-pubapp	4) worker-production-pubapp
#? 4
You have selected service worker-production-pubapp in cluster production-pubapp

Connecting to task (production-pubapp) (869fc2f50ca440938e1e0e25bd1a2db1) in service (worker-production-pubapp)...
869fc2f50ca440938e1e0e25bd1a2db1

The Session Manager plugin was installed successfully. Use the AWS CLI to start a session.


Starting session with SessionId: ecs-execute-command-069b37767401ace92
root@ip-10-128-133-103:/code#
```
