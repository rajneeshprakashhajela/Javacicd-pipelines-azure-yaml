<!-- CICD Pipelines for mule application deployment to cloudhub using GitHub Actions  -->
# Branch Details
There are mainly two branches. Aug/1/2021 :
1. main
2. develop

two entry points for each branches. [ it's better to have two pipeline yaml file for each env rather than combining into one monolithic]
- azure-dev-build-pipeline.yml
- azure-release-build-pipeline.yml

# Azure Environment and Secrets Setup
## Environment
There are few environment created 
1. dev-01
2. qa
3. staging
4. prod
## Environment Secrets
Environment specific variables:  
1. CLOUDHUB_USERNAME
2. CLOUDHUB_PASSWORD

# How to Trigger pipeline
1. Fork this repo 
2. configure your fork and setup azure devops environment and secrets mentioned above
3. Trigger pipeline either manually or github events - PR

# Features
## Mule Application
1. Mule Application compile, build, test, package [Aug/2021]
2. Mule Application release prepare and perform [Aug/2021]
3. CloudHub Deployment using username/password [Aug/2021]
4. Azure devops using yaml file instead of classic UI

# Future Items

