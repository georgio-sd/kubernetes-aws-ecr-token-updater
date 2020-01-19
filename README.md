# Update AWS ECR access token for on-premises kubernetes cluster
AWS Elastic Container Repository requires to rerequest access token every 12 hours in order to use the service with an on-premises kubernetes kluster. This k8s job automatically updates the token every 11 hours.
- aws-upd.yaml - token updater (k8s job)
- scv-acc.yaml - service account for the token updater
- secret-setup - bash script to save aws credentials as a k8s secret
