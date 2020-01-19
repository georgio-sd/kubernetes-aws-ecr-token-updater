# AWS ECR access token updater for on-premises kubernetes cluster
AWS Elastic Container Repository requires to rerequest access token every 12 hours in order to use the service with an on-premises kubernetes kluster. This k8s CornJob automatically updates the token every 11 hours.
- aws-upd.yaml - token updater (k8s CronJob)
- scv-acc.yaml - service account for the token updater
- secret-setup - bash script for saving aws credentials as a k8s secret
