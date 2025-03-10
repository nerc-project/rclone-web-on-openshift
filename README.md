# Rclone Web UI on NERC OpenShift

This is a simple implementation of [Rclone](https://rclone.org/) on OpenShift. It allows you to use its Web interface to easily browse content of endpoints, transfer files,...
The main goal is to provide an easy to use interface to transfer data to/from your environments, from multiple types of endpoints, like S3 Storage or shared file system. It a fast and efficient way to transfer data to/from your data science environment.

On NERC, users will have access to two different images and deployment methods:

- One for use in Red Hat OpenShift AI (RHOAI) within a Data Science Project (DSP).

- One for standalone deployment on any OpenShift environment.

## Deploying Using Data Science Project in the NERC RHOAI

Using your DSP project in the NERC RHOAI, create a new workbench using the existing **Rclone** Notebook image. Set the storage size to the minimum, **100Mi**, as it is only needed to store the configuration of the endpoints. How to deploy using DSP in the NERC RHOAI read [this document](https://nerc-project.github.io/nerc-docs/openshift/storage/Rclone/#deploying-using-data-science-project-dsp-in-the-nerc-rhoai).

Once deployed, launch Rclone from the provided link!

### Source Dockerfile for Building RHOAI Notebook image

In the `odh-rhods/container` folder, you'll find the Dockerfile used to create the RHOAI Notebook image, specifically the **Rclone** image, which is used during the setup of the DSP in the NERC RHOAI.

## Standalone Deployment

How to setup Rclone on NERC OpenShift read [this document](https://nerc-project.github.io/nerc-docs/openshift/storage/Rclone/#deploying-rclone-on-nerc-openshift).

### Source Dockerfile for Building Docker Image

In the `standalone/container` folder you'll find the Dockerfile used to create the container images used in `02-deployment.yaml` at [this line](https://github.com/nerc-project/rclone-web-on-openshift/blob/main/standalone/deploy/02-deployment.yaml#L38).

## Usage

How to properly use Rclone on NERC OpenShift read [this document](https://nerc-project.github.io/nerc-docs/openshift/storage/Rclone/#usage).
