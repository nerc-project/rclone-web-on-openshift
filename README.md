# Rclone Web UI on NERC OpenShift

This is a simple implementation of [Rclone](https://rclone.org/) on OpenShift. It allows you to use its Web interface to easily browse content of endpoints, transfer files,...
The main goal is to provide an easy to use interface to transfer data to/from your environments, from multiple types of endpoints, like S3 Storage or shared file system. It a fast and efficient way to transfer data to/from your data science environment.

On NERC OpenShift, user will be able to use the standalone deployment.

## Standalone Deployment

How to setup Rclone on NERC OpenShift read [this document](https://nerc-project.github.io/nerc-docs/openshift/storage/Rclone/#deploying-rclone-on-nerc-openshift).

## Usage

How to properly use Rclone on NERC OpenShift read [this document](https://nerc-project.github.io/nerc-docs/openshift/storage/Rclone/#usage).

## Source

In the `standalone/container` folder you'll find the Dockerfile used to create the container images used in `02-deployment.yaml` at [this line](https://github.com/nerc-project/rclone-web-on-openshift/blob/main/standalone/deploy/02-deployment.yaml#L38).
