# Pipeline Proccess

we use [CircleCi](https://app.circleci.com/) to create our pipeline to perform our Continuous integration (CI) and Continuous delivery.

[CircleCi](https://app.circleci.com/) will trigger all changes (that are pushed to the github repository) and run the pipeline.

## Pipeline Steps
our pipeline consists of three main jobs:-

### Build
* installing node version 16.18 
* installing backend and frontend dependencies
* pulling updates from the [Github repo](https://github.com/fatmaMGomaa/nd0067-c4-deployment-process-project-starter)
* linting frontend
* building backend and frontend

### Hold
* in this job we ask for approvel to deploy the last version of [Github repo](https://github.com/fatmaMGomaa/nd0067-c4-deployment-process-project-starter) on AWS services S3 Bucket and Elasticbeanstalk


### Deploy
* installing node version 16.18
* installing eb and aws-cli
* installing backend and frontend dependencies
* pulling updates from the [Github repo](https://github.com/fatmaMGomaa/nd0067-c4-deployment-process-project-starter)
* finally we deploy the backened to elasticbeanstalk using eb and deploying frontend to S3 bucket using aws-cli

## Workflows
- Build
- Hold (should be run after build)
- Deploy (should be run after hold)