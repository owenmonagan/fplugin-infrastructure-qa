# pipeline-infrastructure-qa

This repo holds the Kubernetes configuration files for the pipeline application.

## Target Environment

QA

## Usage

Changes pushed to the master branch should trigger the following actions:

  - recursive application of the configuration files located under the kubernetes directory
  - issue a pull request to the [pipeline-infrastructure-production](https://github.com/kelseyhightower/pipeline-infrastructure-production) repo which updates the container image for the pipeline deployment to match the container image deployed to QA.

See the [cloudbuild.yaml](cloudbuild.yaml) file for more details.
