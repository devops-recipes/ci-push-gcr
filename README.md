# Docker Build, Push and Continuous Integration for a Node JS application

[![Run Status](https://api.shippable.com/projects/59005d984f6072070074ce89/badge?branch=master)](https://app.shippable.com/github/devops-recipes/push-docker-hub) [![Coverage Badge](https://api.shippable.com/projects/59005d984f6072070074ce89/coverageBadge?branch=master)](https://app.shippable.com/github/himanshu0503/ci-push-gcr)

![AyeAye](https://github.com/devops-recipes/ci-push-gcr/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI posses and then pushes the image
to GCR

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](wwww.shippable.com)
* Create a Google Cloud [integration](http://docs.shippable.com/platform/integration/gcloudKey/) on shippable to connect your Google Cloud account.
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `gcloud-integration`
* Change the IMAGE_REPO and GCP_PROJECT_ID to point to your repo and Google Cloud Platform project id
* You should be able to run a manual build or webhook build on commit

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/devops-recipes/ci-push-gcr/blob/master/public/resources/images/integration.png)

### CI Console Output
![CI Console Output](https://github.com/devops-recipes/ci-push-gcr/blob/master/public/resources/images/console.png)
