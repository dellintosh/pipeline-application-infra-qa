# pipeline-application-infra-qa

This repo holds the Kubernetes configuration files for the pipeline application.

## Target Environment

QA

## Usage

Changes pushed to the master branch should trigger the following actions:

* recursive application of the configuration files located under the kubernetes directory.
* issue a pull request to the [pipeline-application-infra-production](https://github.com/dellintosh/pipeline-application-infra-production) repo which updates the container image for the pipeline deployment to match the container image deployed to QA.

See the [.drone.yml](.drone.yml) file for more details.