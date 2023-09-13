# Open Science Studio Examples


## What's Here...

These are the compositions to deploy Open Science Studio (OSS) using two different authentication methods, AWS Cognito and Keycloak

## Assumptions

These Crossplane artifacts assume you have a working AWS EKS Cluster deployed and have created the appropriate provider config in your Crossplane installation.  This also assumes you have properly configured your authenication provider (AWS Cognito or Keycloak).  Finally, you'll need both cluster-autoscaler and external DNS deployed in your cluster.

## Required Actions

* Deploy the composite resource definition (xrd) in your environment.
* Customize the composition for your environment, including what container image you would like to run on OSS.  The compositions are commented, so items that need adjusting should be fairly straightforward.
* Deploy the composition using Crossplane.
* Customize your claim with values specific to your environment.
* Deploy your claim.